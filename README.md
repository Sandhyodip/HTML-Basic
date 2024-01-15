# DOCUMENT LINK

`<link>`:  [HTML BASIC DOCUMENTATION BY SANDHYODIP DAS](https://docs.google.com/document/d/1IvktOyOvsvvG3gmwWv8Rve9EQetJZWrUtAUCsKfzo94/edit?usp=sharing)


# What is HTML?

>HTML stands for Hypertext Markup Language. It is used to create websites. It defines page layout / structure of  a web page. It is   not a programming language.

>Let's take a car example.

>HTML => Structure / Layout => Like Car Body (Only Metal)

>CSS => Color, Style, Decoration => Like Car Paint

>JavaScript => Logic => Car Engine + Interior Logic

# Basic Structure of HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
</body>
</html>
```

# From HTML structure we can see

>head & body tags are children of html tag.

>html tag is the parent of head & body tags.

>Most of the HTML elements have opening & closing tags with content in between opening & closing tags.

>Some HTML tags have no content. These are called Empty elements / Void Elements.

>We can use .html or .htm extension for HTML files but .html is recommended.

# Why index.html?

>When we host any website and assign a domain for it, we upload all these files to a server. Now that website can be accessed by entering the domain address you purchased for it (eg: mysite.com) in the URL tab of our browser.

>index.html file is the main page or the Home page of any website. When we enter the domain address of our site, then the server will try to find the file with the name index.html (commonly, if not present it will search for home.html or default.html). If any of these files is present in the directory, then the browser will load that page by default and If not a directory(index) of the files with links will be shown.

# There are two ways to specify the URL in the src attribute:

## 1. Absolute URL

>Links to an external image that is hosted on another website. Example: src="https://www.xyz.com/images/img_nature.jpg".

>External images might be under copyright. If we do not get permission to use it, we may be in violation of copyright laws. In addition, we cannot control external images, they can suddenly be removed or changed.

## 2. Relative URL
>Links to an image that is hosted within the website. Here, the URL does not include the domain name. 

>If the URL begins without a slash, it will be relative to the current page. Example: src="img_girl.jpg". 

>If the URL begins with a slash, it will be relative to the domain. Example: src="/images/img_nature.jpg".

>We should always use relative URLs. They will not break if you change domain. 

# HTML Text Formatting

```html
<b>Bold Text</b>
<i>Italic Text</i>
<u>Underline Text</u>
<big>Big Text</big>
<small>Small Text</small>
<strong>Important Text</strong>
<em>Emphasized Text</em>
<del>Deleted Text</del>
<ins>Inserted Text</ins>
<mark>Marked Text</mark>
<p>C+O<sub>2</sub></p>
<p>A<sup>2</sup>+B<sup>2</sup></p>
<blockquote>Give Some Space in Left</blockquote>
<q>To write a line within quotation</q>
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p> 
<!-- Used to write full form of short words →
<address>  
Written by Sandhyodip Das.<br>
Visit us at:<br>
Noodula.com<br>
Bally 50, Howrah<br>
INDIA
</address>
<!-- Used to write address in different format -->
<p><cite>The Gitanjali </cite > is written by Rabindranath Tagore.</p>
<!-- Used to write a heading in italic or in different format -->
<bdo dir="rtl">This line will be written from right to left</bdo>
<!-- To print a mirror image of a system -->
<code>                                                             
    x = 5;                                                             
    y = 6;                                                                
    z = x + y;                                                  
</code>                                                            
<kbd>Use to define keyboard input (Ctrl + S)</kbd>      
<samp>Use to define sample output from a computer program</samp>
<var>Used to define a variable in programming or in a mathematical expression (x)</var>

```

# We can attach our mail address as a link.
```html
<a href="mailto:sandhyodip17@gmail.com">Send email</a>
```

# HTML picture Element

>The HTML picture element allows us to display different pictures for different devices or screen sizes.

>The picture element contains one or more source elements, each referring to different images through the srcset attribute. This way the browser can choose the image that best fits the current view and/or device.

>Each <source> element has a media attribute that defines when the image is the most suitable.

```html
<picture>
  <source media="(min-width: 650px)" srcset="img_food.jpg">
  <source media="(min-width: 465px)" srcset="img_car.jpg">
  <img src="img_girl.jpg">
</picture>
```
## When to use the Picture Element:

>There are two main purposes for the picture element:

### 1. Bandwidth

>If we have a small screen or device, it is not necessary to load a large image file. The browser will use the first source element with matching attribute values, and ignore any of the following elements.

### 2. Format Support

>Some browsers or devices may not support all image formats. By using the picture element, we can add images of all formats, and the browser will use the first format it recognizes, and ignore any of the following elements.

```html
<picture>
  <source srcset="img_avatar.png">
  <source srcset="img_girl.jpg">
  <img src="img_beatles.gif" alt="Beatles" style="width:auto;">
</picture>
```







