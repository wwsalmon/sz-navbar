# Pure CSS Responsive Navbar

![Demo Gif](demo.gif)

Wide screen -> display navbar items horizontally.
Small screen -> display navbar items vertically in a pull-out hamburger menu.
No JS, just a hidden checkbox and a few lines of CSS magic.

## Demo

See `demo.html` for an example of how to use this, or copy boilerplate html from `boilerplate.html`.

Instructions on how to set things up yourself are below.

## Installation

First, include the CSS file.

There are three options in the `/css` folder of this repo: a standard CSS file if you want to make changes to default values directly, a minified version if you would rather override them in a separate file, and an SCSS file if you're using SCSS, in which case you can override default variables.

For CSS, download either `ww-navbar.css` or `ww-navbar.min.css` and include it in the `<head>` of your HTML document with `<link rel="stylesheet" href="PATH-TO-FILE/ww-navbar.css" type="text/css">`.

For SASS, download `ww-navbar.scss`, put it in your SCSS directory, rename it `_ww-navbar.scss` to prevent it from being compiled, and import it into your stylesheet with `@import 'ww-navbar'`.

## Usage

See to `demo.html` for an example of how to use ww-navbar, or `boilerplate.html` for code to copy+paste into your own project (also shown below).

    <div class="ww-navbar ww-navbar-left"><!-- CHANGE CLASS TO "ww-navbar-right" IF DESIRED -->
        <input type="checkbox" id="ww-navbar-check">
        <label for="ww-navbar-check" class="ww-navbar-hamburger">☰</label><!-- REPLACE WITH YOUR DESIRED HAMBURGER BUTTON -->
        <div class="ww-navbar-items">
            <div class="ww-navbar-item"><span><a href="link1">Item 1</a></span></div><!-- DUPLICATE AS MANY OF THESE AS DESIRED -->
        </div>
    </div>