# Website Performance Optimization (Udacity)

## Summary

The goal of the project is to improve page performance. For this we need to achieve at least 90 points in PageSpeed ​​Insights and run the page at 60 fps.

In this repository you will find a minified version of each css and javascript provided, wich I made to implement later.


To run the app, you can download [here](https://github.com/alexmonteirov/frontend-nanodegree-mobile-portfolio/archive/master.zip) or click [here](https://alexmonteirov.github.io/frontend-nanodegree-mobile-portfolio/) to see app hosted on GitHub Pages.

### Part 1: Optimize PageSpeed Insights score for index.html

1. Used the optimized images that PageSpeed Insights have provided.
2. Move external CSS files 'style.css' and 'print.css' to inline style in index.html.
3. Async javascript links in index.html.
4. Used Web Font Loader to prevent render blocking by Google Fonts font load.

PageSpeed Insights score:
* Mobile: 96/100
* Desktop: 95/100

### Part 2: Optimize Frames per Second in pizza.html

#### Optimizing (Not required)

1. Moved external CSS 'style.css' to inline style in index.html.
2. Minified 'bootstrap-grid.min.css' that was provided.

PageSpeed Insights score:
* Mobile: 89/100
* Desktop: 95/100

#### Scrolling

* Change pizzas loaded from 200 to 30.

* Moved ```(document.body.scrollTop / 1250)``` into a new variable outside the for loop.

#### Pizza Resizes

1. Removed variables: ```oldwidth```, ```windowwidth```, ```oldsize```, ```newsize```, and ```dx```.

2. Changed ```newwidth``` values inside switch function with percentages values.

3. New ```randPizzas``` and ```numPizzas``` variables to simplify the for loop.

4. Moved ```pizzasDiv``` variable outside the for loop.
