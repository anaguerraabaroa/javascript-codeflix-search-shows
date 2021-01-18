![Codeflix Search Engine Banner](https://pro.sony/s3/2017/04/08151948/main-banner_1600x450.jpg)

# **CodeflixSearchEngine**

Module 2 final project of the Adalab Digital Frontend Development Bootcamp.

This is a responsive TV shows search engine web app developed with [<img src = "https://img.shields.io/badge/-HTML5-E34F26?style=flat&logo=html5&logoColor=white">](https://html.spec.whatwg.org/) [<img src = "https://img.shields.io/badge/-CSS3-1572B6?style=flat&logo=css3&logoColor=white">](https://www.w3.org/Style/CSS/) and [<img src = "https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black">](https://www.ecma-international.org/ecma-262/)

## **Quick start guide**

Instructions to start this project:

### **Pre-requirements**

This project runs with Adalab Starter Kit [**here**](https://github.com/Adalab/adalab-web-starter-kit).

In order to use this kit it is needed to previously install [<img src="https://img.shields.io/badge/-node.js-339933?style=flat&logo=node.js&logoColor=white">](https://nodejs.org/es/), [<img src="https://img.shields.io/badge/-Git-F05032?style=flat&logo=git&logoColor=white">](https://git-scm.com/) and [<img src="https://img.shields.io/badge/-Gulp.js-CF4647?style=flat&logo=gulp&logoColor=white">](https://gulpjs.com/) to automate tasks and control project versions.

### **Installation**

1. Clone repository
2. Open a terminal
3. Run `npm install` on the terminal to install local dependencies

### **Run project**

Run `npm start` on the terminal:

1. Open the project on the browser using a local server.
2. Refresh browser everytime files contained in `/src` folder are updated.
3. Compiled files contained in `/src` folder and copy them in `/public` folder in order to be prepared for production environment.

### **Updating**

1. Run these commands to update changes on the project:

```
git add -A
git commit -m "Message commit"
git push
```

2. Run `npm run docs` to create `/docs` folder and the production environment version.

3. Run again commands on step 1 to update changes on the project.

4. Project **[URL](https://anaguerraabaroa.github.io/CodeflixSearchEngine/)** is also available on GitHub Pages.

## **Exercise features**

- TV shows search form with an input to enter show name and a button to send the request to the [**API**](http://api.tvmaze.com/search/shows?q=girls)
- Search results list with the name and an image of the show. If the show has not an image, it is shown a default image
- Select favourite shows by clicking on the show and changing background colour. Selected favourite shows remain although user do a new search
- Favourite shows list under search form
- Reset button to remove all shows from favourites list
- Close button on each favourites card to remove shows individually
- Set favourite shows on LocalStorage to get data when app is run

## **Folder Structure**

```
CodeflixSearchEngine
├── docs
├── node_modules
├── public
├── src
│   ├── html
│   │   ├── partials
│   │   │   ├── footer.html
│   │   │   ├── header.html
│   │   │   ├── hero.html
│   │   │   ├── main.html
│   │   │   ├── section-favourites.html
│   │   │   ├── section-results.html
│   │   │   └── section-search.html
│   │   └── index.html
│   ├── images
│   │    ├── default_image.jpg
│   │    ├── favicon.png
│   │    ├── landing_desktop.png
│   │    ├── landing_mobile.png
│   │    ├── landing_tablet.png
│   │    └── hero.jpg
│   ├── js
│   │    ├── 01search.js
│   │    ├── 02favourites.js
│   │    ├── 03localStorage.js
│   │    ├── 04reset.js
│   │    ├── 05removeFavourites.js
│   │    └── 06main.js
│   └── scss
│       ├── core
│       │   ├── _reset.scss
│       │   └── _variables.scss
│       ├── layout
│       │   ├── _footer.scss
│       │   ├── _header.scss
│       │   ├── _hero.scss
│       │   ├── _section-favourites.scss
│       │   ├── _section-results.scss
│       │   └── _section-search.scss
│       ├── pages
│       │   └── _index.scss
│       └── main.scss
├── .browserslistrc
├── .csscomb.json
├── .eslintrc.json
├── .gitignore
├── config.json
├── debug.log
├── gulp-flow.png
├── gulpfile.js
├── LICENSE
├── package-lock.json
├── package.json
├── README.md
└── robots.txt
```

## **Listeners and functions**

### **Search**

- **Event listener:** btnElement.addEventListener("click", getData)
- **Get data from API:** function getData()
- **Render search result list:** function paintData()

### **Favourites**

- **Event listener:** function listenFavourites()
- **Handle favourites array:** function favouriteShows(event)
- **Render favourite shows list:** function paintFavShows()

### **LocalStorage**

- **Set data in LocalStorage:** function setLocalStorage()
- **Get data from LocalStorage:** function getLocalStorage()

### **Reset**

- **Event listener:** resetBtn.addEventListener("click", handleReset)
- **Handle reset:** function handleReset()

### **Remove shows from favourite shows list**

- **Event listener:** function listenRemoveBtn()
- **Remove shows from favourite shows list individually:** function removeFavShow(event)

## **Result**

![Mobile version](./src/images/landing_mobile.jpg) ![Tablet version](./src/images/landing_tablet.jpg) ![Dektop version](./src/images/landing_desktop.jpg)

## **License**

This project is licensed under [**MIT License**](https://spdx.org/licenses/MIT.html).
