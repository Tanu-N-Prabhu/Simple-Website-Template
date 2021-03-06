<h1 align = "center">Simple-Website-Template</h1>

<p align = "center">
<img src = "https://github.com/Tanu-N-Prabhu/Simple-Website-Template/blob/main/Img/web-design-background_1300-39.jpg">
</p>

## Objective

<p align = "justify">In this repository, you learn to develop a static website from scratch. There is a bonus at the end of this tutorial, which is you will understand the essence of GitHub Pages and its free hosting capability. By completing this tutorial, you will have a fully functional website template deployed on the internet. You can further extend this template to build a portfolio for yourself, friends/family, or anybody needs a portfolio.</p>

> Prior to this tutorial, one must have <b>minimal understanding</b> on HTML, CSS, Bootstrap and JavaScript. 


# Steps to successfully build a functional website

Below are the steps to build a complete functional website.

1. Create both header (Navigation Bar) and footer using Inheritance (Jquery).
2. Create a <b>"Home"</b> page and other options page as needed.
3. ....



## Simple Responsive Navigation bar

<p align = "justify">While designing a navigation bar, no matter what you do and why you do, but please try to make it responsive. Because not all users will open your website on Laptops or computer but there are some users who prefer small acpect ratio devices too. So always make you navigation responsive.</p>

### How to do?

The answer is pretty trivial, use Bootstrap. This is why bootstrap is used, to create responzive websites. Now to do this you will be just using some of its libraries to inculcate responsiveness.

#### Navbar Inheritance

<p align = "justify">Now this is one of the best practices to implement. For example, it is not a good idea to put the same chunk of navigation bar or footer in every single page. Suppose if you want to change a particular option name or fix the typo, then image the number or times you need to reciprocate your code. Rather, why not use Navbar inheritance. This means in simple words, write the code once and use it in many pages. Once you update a single option in the main page, then automatically every page would be updated.</p>
##### 1. For this we need to use `JQuery` library



```html
<!-- Used for inheriting -->
<script src="https://code.jquery.com/jquery-1.10.2.js"></script>
```


##### 2. Place the `id` inside the `div` inside the `body` of HTML

Create a random `id` for the navigation bar and footer

```html
<!-- Navigation bar ---->
<!-- Inheriting the navbar from header.html-->
<div id = "nav-placeholder"></div>          
<!-- Make sure you place it in a div tag -->
```


##### 3. Load the `navBar` page using Javascript

Make sure the `id` in both cases match. Also include the link of your navigation bar page inside the `load()`

```Javascript
$(function(){
    $("#nav-placeholder").load("navBar.html");
    });
```


> <b>Note</b>: Make sure you add all the necessary navigation bar code in a sperate file called `navBar.html` and its CSS file as `navBarStyle.css`. Now you can put the above in any of the HTML pages to get the navigation bar.


### Navigation bar 

Executed on my Laptop - HP Elitebook

<img src = "https://github.com/Tanu-N-Prabhu/Simple-Website-Templates/blob/main/Img/nav1.PNG">

Executed on the emulator - iPhone X

<img src = "https://github.com/Tanu-N-Prabhu/Simple-Website-Templates/blob/main/Img/nav2.PNG">

### Footer 

Executed on my Laptop - HP Elitebook

<img src = "https://github.com/Tanu-N-Prabhu/Simple-Website-Templates/blob/main/Img/footer.PNG">


