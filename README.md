# Google Chrome Extension Popup with Framework7

## About Framework7 

Framework7 - is a free and open source mobile HTML framework to develop hybrid mobile apps or web apps with iOS & Android native look and feel. It is also an indispensable prototyping apps tool to show working app prototype as soon as possible in case you need to.

The main approach of the Framework7 is to give you an opportunity to create iOS & Android apps with HTML, CSS and JavaScript easily and clear. Framework7 is full of freedom. It doesn't limit your imagination or offer ways of any solutions somehow. Framework7 gives you freedom!

Framework7 is not compatible with all platforms. It is focused only on iOS and Google Material design to bring the best experience and simplicity.

Framework7 is definitely for you if you decide to build iOS or Android hybrid app (PhoneGap) or web app that looks like and feels as great native iOS and Google Material apps.

[Framework7 Website](https://framework7.io/)

## About this Repository 

This repository allows you to use the same code of your FW7 applications in the Google Chrome Extension Popup. 

Use cases can be multiple and varied, you can increase the number of users who use your application with minimum effort, with very few tricks. 

In fact you have to add only one  `<div>` in your index.html, and the magic will be done. 

## How to 

Check the `index.html` file: 

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Google Chrome Extension Popup With Framework7</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, minimum-scale=1, user-scalable=no, minimal-ui, viewport-fit=cover">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
    <link rel="stylesheet" href="./lib/framework7/css/framework7.min.css">
    <link rel="stylesheet" href="./css/framework7-icons.css">
    <link rel="stylesheet" href="./css/chrome-extension.css">
</head>
<body class="color-theme-blue">
    <!-- This is the app.root -->
    <div id="app">
        <!-- Add inside id="app"  a div with the class="app-container" -->
        <div class="app-container">
            <!-- Initialize your app inside view view-main -->
            <div class="view view-main"></div>
        </div> <!-- / .app-container -->
    </div> <!-- / .app -->

    <script type="text/javascript" src="./lib/framework7/js/framework7.min.js"></script>
    <script type="text/javascript" src="./js/app.js"></script>
</body>
</html>
```

As you can see, is very simple. The first thing to do is to add `chrome-extension.css` in your `index.html` file, after the **Framework7** files. After that you have to add`<div class="capp-container">` container after your `app.root` (usually is `<div id="app">`). This sub container allow your app to be visualize correctly in the popup of Google Chrome.