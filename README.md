# Simple-Website-Templates

## Simple Responsive Navigation bar

While designing a navigation bar, no matter what you do and why you do, but please try to make it responsive. Because not all users will open your website on Laptops or computer but there are some users who prefer small acpect ratio devices too. So always make you navigation responsive. 

### How to do?

The answer is pretty trivial, use Bootstrap. This is why bootstrap is used, to create responzive websites. Now to do this you will be just using some of its libraries to inculcate responsiveness.

#### Navbar Inheritance

Now this is one of the best pratices to implement. For example, it is not a good idea to put the same chunk of navigation bar or fotter in every single page. Suppose if you want to change a particular option name or fix the typo, then image the number or times you need to reciprocate your code. Rather why not use NanBar inheritance. This means in simple words, write the code once and use it in many pages. Once you update a single option in the main page, then automatically every page would be updated.

##### 1. For this we need to use `JQuery` library



```html
<!-- Used for inheriting -->
<script src="https://code.jquery.com/jquery-1.10.2.js"></script>
```


##### 2. Place the `id` inside the `div` inside the `body` of HTML

Create a random `id` for the navigation bar

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


### Result

Executed on my Laptop - HP Elitebook

<img src = "https://github.com/Tanu-N-Prabhu/Simple-Website-Templates/blob/main/Img/nav1.PNG">

Executed on the emulator - iPhone X

<img src = "https://github.com/Tanu-N-Prabhu/Simple-Website-Templates/blob/main/Img/nav2.PNG">




