# Website Performance Optimization

This project aims to optimize a provided website with a number of optimization- and performance-related issues so that it achieves a target PageSpeed score and runs at 60 frames per second. As web applications become increasingly interactive and accessed on a variety of devices there are a variety of opportunities in which performance issues can hinder the user experience. This project presents a number of those performance issues.

Open and view the Project using the .zip file provided or at my [Github Repository](https://github.com/madhur-taneja/Web-Optimization-Checking).

The project is also hosted on [GitHub](https://madhur-taneja.github.io/Web-Optimization-Checking/)

## Table of Contents
- [Getting Started](#getting-started)
	- [Tools Required](#tools-required)
	- [Installation](#installation)
- [Development](#development)
  - [Part 1: Optimize PageSpeed Insights score for index.html](#part-1-optimize-pagespeed-insights-score-for-indexhtml)
  - [Part 2: Optimize Frames per Second (FPS) in pizza.html](#part-2-optimize-frames-per-second-fps-in-pizzahtml)
- [Running the App](#running-the-app)
- [References](#references)

## Getting started

The project will be evaluated by a Udacity code reviewer according to the Web Optimization project [rubrics](https://review.udacity.com/#!/projects/2735848561/rubric)

### Tools required:

* [CSS Minifier](https://cssminifier.com/)
* [JS Minifier](https://javascript-minifier.com/)
* [Kraken.io](https://kraken.io/) and [Optimizilla](http://optimizilla.com/)
* [PageSpeed Tools](https://developers.google.com/speed/pagespeed/insights/)

### Installation

No additional installation is required for this project

## Development

### Part 1: Optimize PageSpeed Insights score for index.html

* The aim of this project was to optimize `index.html` to a pageinsight speed score above 90.
* My score was: 95 for Mobile and 96 for Desktop version.

#### Step 1: Optimizing `index.html`
> Unlinking style.css and making it internal after minifying it. </br>
> Using media query "print" on print.css. </br>
> Shifting script tags from head to end of body and using async attribute on them.

### Part 2: Optimize Frames per Second (FPS) in pizza.html
* The aim of this project was to optimize `pizza.html` to 60 fps scrolling speed.
* And to reduce the `pizzaResizeTime` less than 5ms.

#### Step 1: Optimizing `pizza.html`
> Shifting script tags from head to end of body.

#### Step 2: Optimizing `main.js`
> Minified js for arrays. </br>
> Changes in changePizzaSizes()
* Declaring rPC and dx outside the loop as it was being declared again and again.
> Changes in `UpdatePosition()` function.
* Declaring phase outside the loop as it was being declared again and again.
> Changes in `document.addEventListener()`.
* Reducing the number of times the loop runs as image will be generated lesser number of times.

## Running the App:

* Open the project through the `hosting link` provided above or the `.zip` file provided and extract the files. 
  * Open `index.html` in the browser of your choice.
  * Open `views/pizza.html`.
    > `pizza.html` can also be opened through `Cam's Pizzeria` link in `index.html`.


## References

* [Web Optimization Course](https://classroom.udacity.com/courses/ud884)
