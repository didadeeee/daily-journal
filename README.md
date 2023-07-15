Hello! I am learning to create a React App, 'GPT3', coding along with [JavaScript Master](https://www.youtube.com/watch?v=F627pKNUCVQ).

## Key Learnings: 
- learning the practical ways of setting up react app
- practice on my css skills
- get familiarise on the file organization

## Getting Started:

- create a git repository on github
- connect the local environment using git desktop
- in the terminal - type npx create-react-app ./
- update gitignore with [Toptal](https://www.toptal.com/developers/gitignore/)
- remove src folder and create a new src folder
- create index.js, insert code below -

```
import React from 'react';
import ReactDOM from 'react-dom';

import App from './App';

ReactDOM.render(<App />, document.getElementById('root'));
```

- npm install react-icons

**TIPS** _type rsf to get a functional component (depending on your extension installed)_

- create App.js, insert your code

```
import React from 'react';

function App(props) {
    return (
        <div>
            <h1>Daily Journal</h1>
        </div>
    );
}

export default App;
```

**TIPS** _git push whenever (git add -A, git status, git commit -m 'initial environment', git push)_

- npm start to start your server
- start creating components & containers folder
- create index.js in the components/containers folder, insert code below -

```
export { default as Blog } from './blog/Blog';
export { default as Features } from './features/Features';
export { default as Footer } from './footer/Footer';
export { default as Header } from './header/Header';
export { default as Possibility } from './possibility/Possibility';
export { default as WhatGPT3 } from './whatGPT3/WhatGPT3';
```

- insert initial styling in App.css

```
* {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
    scroll-behavior: smooth;
}

body {
     background: var(--color-bg);
}

and more..
```

- insert initial styling in index.css

```
@import url('https://fonts.googleapis.com/css2?family=Manrope:wght@200;300;400;500;600;700;800&display=swap');

:root {
  --font-family: 'Manrope', sans-serif;

  --gradient-text: linear-gradient(89.97deg, #AE67FA 1.84%, #F49867 102.67%);
  --gradient-bar: linear-gradient(103.22deg, #AE67FA -13.86%, #F49867 99.55%);

  --color-bg: #040C18;
  --color-footer : #031B34;
  --color-blog: #042c54;
  --color-text: #81AFDD;
  --color-subtext: #FF8A71;
}
```

- media query, 700px for middle size device

```
@media screen and (max-width: 700px) {
    .section__padding {
      padding: 4rem;
    }

    .section__margin {
      margin: 4rem;
    }
  }
```

- media query, 550px for middle size device

```
  @media screen and (max-width: 550px) {
    .section__padding {
      padding: 4rem 2rem;
    }

    .section__margin {
      margin: 4rem 2rem;
    }
  }
```

## Resources:

Markdown Cheatsheet: [Moodle](https://docs.moodle.org/402/en/Markdown#:~:text=Bullet%20point%20lists%20can%20be,and%20should%20not%20be%20forgotten.)<br>
Gradient Generator: [Angry Tools](https://angrytools.com/gradient/), [Online Tutorial](https://www.youtube.com/watch?v=F627pKNUCVQ) (30:54 onwards) <br>
CSS Animation: [Animista](https://animista.net/)<br>
CSS BEM Naming: [CSS Wizardry](https://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/)<br>
CSS Flexbox Tutorial: [Sharkcoder](https://sharkcoder.com/layout/flexbox)<br>
Responsive and Optimised Image: [Sharkcoder](https://sharkcoder.com/images/responsive-images)<br>
