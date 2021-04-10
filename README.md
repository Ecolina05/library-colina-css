# COLINA CSS

Colina CSS is a CSS framework **based on utilities**.
___
## Table of contents

- [Quick Install](#quick-install)
- [What's included](#whats-included)
- [Adding in Angular projects](#adding-in-angular-projects)
- [Creator](#creator)

## Quick Install

- **npm**
```
npm i colina-css
```
## What's included 

Within the download, you will find the directory with a single minified style file. Kind of:

```
dist
    ├── css
        └── colina.min.css
```

## Adding in Angular projects
Adding Colina CSS to an angular project is as easy as just adding the **colina.min.css** to **angular.json** file.<br>
So, open angular.json file, inside of projects → project-name → architect → styles. Add a new item to it with the path for colina.min.css.
```
...
    "styles": [
        "node_modules/colina-css/dist/css/colina.min.css",
        "src/styles.css"
    ],
...
```

## Creator

**Ernesto Colina Jiménez**

- <https://github.com/ecolina05>
- <https://www.linkedin.com/in/ecolina05/>