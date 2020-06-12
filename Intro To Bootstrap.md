# BOOTSTRAP

[Intro Page For Bootstrap Website](https://getbootstrap.com/docs/4.4/getting-started/introduction/)
Bootstrap is the most popular HTML, CSS, and JavaScript framework for developing responsive, mobile first projects on the web. OR Bootstrap is a giant collection of handy, reusable bits of code written in HTML, CSS, and JavaScript.

# ADDING BOOTSTRAP TO YOUR PROJECT

Since bootstrap are collection of css and javascript file they should be added to out html file. There are two ways to add bootstrap to a project.

##  USING BOOTSTRAP CDN

[Link For Bootstrap CDN](https://getbootstrap.com/docs/4.5/getting-started/download/#bootstrapcdn)
This method involves adding cached version of Bootstrap’s compiled CSS and JS to your project.There is no point of adding its syntax to this notes as it changes with different version.

## DOWNLOADING COMPILED VERSION OF BOOTSTRAP

[Link For Complied Version of CSS and JS](https://getbootstrap.com/docs/4.5/getting-started/download/#compiled-css-and-js)
Using this method bootstrap file can be easily added to project by using standard syntax to add js and css file.

# BOOTSTRAP CLASSES

[W3's Bootstrap 4 Classes definition](https://www.w3schools.com/bootstrap4/bootstrap_ref_all_classes.asp)
[Bootstrap Docs For Bootstrap components](https://getbootstrap.com/docs/4.0/components/)
Bootstrap 4 contains almost 1000 unique classes , so it's a waste to make a comprehensive notes on bootstrap classes. But there are some sites which provide definition for all classes like `w3school` and bootstrap's official documentation  but these links becomes obsolete as new version arrives !!


# IMPORTANT BOOTSTRAP CSS CLASSES

1. Forms and Inputs - [W3 Link for Bootstrap's Forms ](https://www.w3schools.com/bootstrap4/bootstrap_forms.asp)
2. Jumbotron - [Bootstrap Docs For Jumbotron](https://getbootstrap.com/docs/4.0/components/jumbotron/) Jumbotron helps us to showcase key marketing messages on our site.
3. Nav Bars - [Bootstrap Docs For Nav Bar](https://getbootstrap.com/docs/4.0/components/navbar/)

# NAV BAR

[Bootstrap Docs For Nav Bar](https://getbootstrap.com/docs/4.0/components/navbar/)
Nav Bar provides easy navigation between different external and internal component of websites which includes support for branding, navigation, and more, including support for collapse plugin.

For better mobile support bootstrap provide `hamburger` style to minimize nav bar for mobile screen size but it includes javascript codes and javascript framework such as jquery .

Code To include Hamburger style without javascript code :

```
<script src="https://code.jquery.com/jquery-3.4.1.slim.min.js" integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n" crossorigin="anonymous"></script>
	<script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
	<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>

```

# BOOTSTRAP ICONS

[Bootstrap Icon's](https://icons.getbootstrap.com/)
Bootstrap Icons are designed to work with Bootstrap components, from form controls to navigation. Bootstrap Icons are SVGs, so they scale quickly and easily and can be styled with CSS.
Method to include bootstrap icon using svg.

```
<svg class="bi bi-chevron-right" width="32" height="32" viewBox="0 0 20 20" fill="currentColor" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6.646 3.646a.5.5 0 01.708 0l6 6a.5.5 0 010 .708l-6 6a.5.5 0 01-.708-.708L12.293 10 6.646 4.354a.5.5 0 010-.708z" clip-rule="evenodd"/></svg>

```
# BOOTSTRAP BORDERS

[Bootstrap Borders's](https://getbootstrap.com/docs/4.5/utilities/borders/)
Most of the info in provided in bootstrap docs but there is also a very intuitive way of adding border's in bootstrap -

```
<h1 class="border border-left-0">Give me border</h1>
```
This will introduce border on all sides except left side since it is assigned zero.

# FLEXBOX
[Info about Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flexbox-background)
Flexbox Layout help us to provide a efficent way to lay out,align and distribute space among items in an contianer,even when their sizes is unknow and or/ dynamic .
