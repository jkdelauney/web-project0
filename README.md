# Project 0

Web Programming with Python and JavaScript

This is the first project in the CS50 Web Dev program.

I've done most of this before but it's been ages, so it'll be a good refresher.

### Requirements

- [x] Website must contain at least four different .html pages and it should be possible to get from any page on the website to any other page by following one or more hyperlinks.
- [x] Website must include at least one list (ordered or unordered), at least one table, and at least one image.
- [x] Website must have at least one stylesheet file.
- [x] Stylesheet(s) must use at least five different CSS properties and at least five different types of CSS selectors. You must use the #id selector at least once and the .class selector at least once.
- [x] Stylesheet(s) must include at least one mobile-responsive `@media` query, such that something about the styling changes for smaller screens.
- [x] You must use Bootstrap 4 on your website, taking advantage of at least one Bootstrap component, and using at least two Bootstrap columns for layout purposes using Bootstrap’s grid model.
- [x] Stylesheets must use at least one SCSS variable, at least one example of SCSS nesting, and at least one use of SCSS inheritance.

#### View

[View current Website](https://jkdelauney.github.io/web-project0/)

###### Project Description

As this project did not require any actual functionality I did a simple write up using an old personal website as inspiration.

Each page contains a <nav> and <footer>. The nav contains the links to each page and the active page's link has the bootstrap disabled class applied. A :hover selector is used to set the color of hovered links to black.

The footer is pinned to the bottom of the page and is hidden using bootstraps built-in functionality when the viewport is reduced in width to around the size of a mobile phone. The footer also contains a link which is itself an image.

The main content on each page is contained in a bootstrap jumbotron. The header in each page's jumbotron is resized from 3.5rem which is applied using bootstrap's .display-4 class to 2.5rem using a `@media` query.

Finally on all pages text highlighting is modified using the ::selection selector to set the highlighted text to gray and background to purple.

###### index.html

This page is a simple landing page and all of the features are those that exist on all pages.

###### about.html

The About page includes ai bootstrap styled table and text in it's jumbotron which are layed out using bootstrap col classes so that the text moves under the table when the viewport gets smaller.

###### projects.html

The Projects page also uses col classes to layout text along side an unordered list styled using bootstrap. The first item in this list has an underline text-decoration applied using an id selector.

###### plans.html

The Plans page is a sibling of the Projects page, using the same bootstrap features and css overrides.

###### css/overrides.scss

This file contains all styling that is not provided by bootstrap, and is headed by two rows of three dashes to trigger Jekyll on GitHub Pages as I was not getting the .scss file to render without them.

###### css/build

A simple shell script to strip out the leading dashes from the .scss file so that the local Sass install could build the .scss file without the dashes appearing in the resulting .css file.
