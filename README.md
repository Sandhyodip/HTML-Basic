# DOCUMENT LINK

`<link>`:  [HTML BASIC DOCUMENTATION BY SANDHYODIP DAS](https://docs.google.com/document/d/1IvktOyOvsvvG3gmwWv8Rve9EQetJZWrUtAUCsKfzo94/edit?usp=sharing)


# WHAT IS HTML?

>HTML stands for Hypertext Markup Language. It is used to create websites. It defines page layout / structure of  a web page. It is   not a programming language.

>Let's take a car example.

>HTML => Structure / Layout => Like Car Body (Only Metal)

>CSS => Color, Style, Decoration => Like Car Paint

>JavaScript => Logic => Car Engine + Interior Logic

# BASIC STRUCTURE OF HTML

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

|  HTML STRUCTURE | DESCRIPTION |
| ------------- | ------------- |
| &lt;!DOCTYPE html&gt;  | Specifies that this is an HTML 5 Document  |
| &lt;html lang="en"&gt;  | Root of an HTML page & language is English.  |
| &lt;head&gt;  | Contains page metadata. Information about some already existing data.  |
| &lt;meta charset="UTF-8"&gt;  | Represents any character in the unicode standard.  |
| &lt;meta http-equiv="X-UA-Compatible" content="IE=edge"&gt;  | It is used for compatibility with old microsoft browsers. It allows web authors to choose what version of Internet Explorer the page should be rendered as.  |
| &lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;  | Not all devices are the same width. We should make sure that our pages work well in a large variation of screen sizes and orientations. Mainly it is used for responsiveness.  |
| &lt;title&gt; Document &lt;/title&gt;  | Contains Title. Defines the page information.  |
| &lt;/head&gt;  | End tag of head tag  |
| &lt;body&gt;   | The main part of the page i.e rendered by the browser. Here we write all the codes for required structure.  |
| &lt;/body&gt;  | End tag of body tag  |
| &lt;/html&gt;  | End tag of html tag  |

# HTML TAG

>Tag is the component that is used to design the structure of a website. Basically it is a container of more tags or content.

>Example: body, head, h1, p

# HTML ELEMENT

>Tag including content is called an HTML element.

```html
<tag> Content </tag> 
<h1>This is header</h1>
<startTag>Content</endTag>
```

### FROM HTML STRUCTURE WE CAN SEE:

>head & body tags are children of html tag.

>html tag is the parent of head & body tags.

>Most of the HTML elements have opening & closing tags with content in between opening & closing tags.

>Some HTML tags have no content. These are called Empty elements / Void Elements.

![](images/HTML_FLOW.png)

>From the above figure we can see how the html document is being rendered by the browser.

>We can use .html or .htm extension for HTML files but .html is recommended.

>File name for the html file must be index.html. We can give other names like view.html but index.html is recommended.

# WHY index.html?

>When we host any website and assign a domain for it, we upload all these files to a server. Now that website can be accessed by entering the domain address you purchased for it (eg: mysite.com) in the URL tab of our browser.

>index.html file is the main page or the Home page of any website. When we enter the domain address of our site, then the server will try to find the file with the name index.html (commonly, if not present it will search for home.html or default.html). If any of these files is present in the directory, then the browser will load that page by default and If not a directory(index) of the files with links will be shown.

![Example Image](images/folder_structure.png)

>Image: Directory of files with hyperlink. Source: Google

>Because, the server doesn’t know which file to open first. So the name of all the files with links will be listed instead of any particular homepage.

>For example, when we enter avast.com in the URL tab, it will take us to the homepage of Avast website because that page is named as index.html.

>That’s why we should name our home page as index.html to avoid any error.

# CASE SENSITIVITY

HTML is case insensitive language. &lt;H1&gt; and &lt;h1&gt; tags are the same.

# HTML ATTRIBUTE

>It is used: 

1. to add more or additional information corresponding to an HTML Tag.
2. It is always specified in the start tag
3. It is usually in name/value pairs like: name="value".

```html
<a href=’https://noodula.com/’> Click Here </a>
```

>Here href is the attribute. It is providing an additional url link corresponding to the anchor tag.

```html
<img src="img_girl.jpg">
```

>Here src attribute is used for image url corresponding to the image tag.

# THERE ARE TWO WAYS TO SPECIFY THE URL IN HTML

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

# DAILY ROUTINE TABLE STRUCTURE

```html
<h1 align="center">Daily Routine</h1>                       
    <table align="center" cellspacing="0" border="5">             
        <tr>                                                          
            <td align="center" height="50" width="100"><b>Day/Period</b></td>                            
            <td align="center" height="50" width="100"><b>I<br>9:30-10:20</b></td>                       
            <td align="center" height="50" width="100"><b>II<br>10:20-11:10</b></td>                     
            <td align="center" height="50" width="100"><b>III<br>11:10-12:00</b></td>                    
            <td align="center" height="50" width="100"><b>12:00-12:40</b></td>
            <td align="center" height="50" width="100"><b>IV<br>12:40-1:30</b></td>                      
            <td align="center" height="50" width="100"><b>V<br>1:30-2:00</b></td>
            <td align="center" height="50" width="100"><b>VI<br>2:00-3:10</b></td>
            <td align="center" height="50" width="100"><b>VII<br>3:10-4:00</b></td>                    
         </tr>                                                         
         <tr>
            <td align="center" height="50" width="100"><b>Monday</b></td> 
            <td align="center" height="50" width="100"><b>English</b></td>
            <td align="center" height="50" width="100"><b>Math</b></td>
            <td align="center" height="50" width="100"><b>Chemistry</b></td>
            <td rowspan="3" align="center" height="50" width="100"><b>L<br>U<br>N<br>C<br>H</b></td>                 
            <td colspan="3" align="center" height="50" width="100"><b>Lab</b></td>                                   
            <td align="center" height="50" width="100"><b>Physics</b></td> 
        </tr>                                                         
        <tr>                                                          
            <td align="center" height="50" width="100"><b>Tuesday</b></td>      
            <td colspan="3" align="center" height="50" width="100"><b>Lab</b></td>                                   
            <td align="center" height="50" width="100"><b>English</b></td>  
            <td align="center" height="50" width="100"><b>Math</b></td>   
            <td align="center" height="50" width="100"><b>Chemistry</b></td> 
            <td align="center" height="50" width="100"><b>Sports</b></td> 
        </tr>                                                        
        <tr>                                                          
            <td align="center" height="50" width="100"><b>Wednesday</b></td> 
            <td align="center" height="50" width="100"><b>Bengali</b></td> 
            <td align="center" height="50" width="100"><b>English</b></td> 
            <td align="center" height="50" width="100"><b>Math</b></td>   
            <td align="center" height="50" width="100"><b>Chemistry</b></td> 
            <td colspan="3" align="center" height="50" width="100"><b>Lab</b></td>                                 
        </tr>                                                     
    </table>
```

# URL Encoding

> URLs can only be sent over the Internet using the ASCII character-set. If a URL contains characters outside the ASCII set, the URL has to be converted. URL encoding converts non-ASCII characters into a format that can be transmitted over the Internet and replaces non-ASCII characters with a "%" followed by hexadecimal digits.         URLs cannot contain spaces. URL encoding normally replaces a space with a plus (+) sign, or %20. 

# URL Web Storage API
> With web storage, web applications can store data locally within the user's browser. Before HTML5, application data had to be stored in cookies, included in every server request. Web storage is more secure, and large amounts of data can be stored locally, without affecting website performance.  

>Unlike cookies, the storage limit is far larger (at least 5MB) and information is never transferred to the server.    

>Web storage is per origin (per domain and protocol). All pages, from one origin, can store and access the same data.

#### HTML web storage provides two objects for storing data on the client:

1. window.localStorage - Stores data with no expiration date
2. window.sessionStorage - Stores data for one session (Data is lost when the browser tab is closed)
                
>The localStorage object stores the data with no expiration date. The data will not be deleted when the browser is closed, and will be available the next day, week, or year.

```javascript
localStorage.setItem("lastname", "Smith");
document.getElementById("result").innerHTML = localStorage.getItem("lastname");
```

>The sessionStorage object is equal to the localStorage object, except that it stores the data for only one session. The data is deleted when the user closes the specific browser tab.

```javascript
sessionStorage.setItem('mother','Mridula Das');
document.getElementById('demo').textContent=sessionStorage.getItem('mother');
```

# URL Web Workers API

>A web worker is a JavaScript running in the background, without affecting the performance of the page. 

>When executing scripts in an HTML page, the page becomes unresponsive until the script is finished. A web worker is a JavaScript that runs in the background, independently of other scripts, without affecting the performance of the page. 

>We can continue to do whatever we want: clicking, selecting things, etc., while the web worker runs in the background.

# URL SSE API

>Server-Sent Events (SSE) allow a web page to get updates from a server.

>This was also possible before, but the web page would have to ask if any updates were available. With server-sent events, the updates come automatically.

```php
<?php
header('Content-Type: text/event-stream');
header('Cache-Control: no-cache');

$time = date('r');
echo "data: The server time is: {$time}\n\n";
flush();
?>
```

## Setting Headers:

1. header('Content-Type: text/event-stream'): 

>This header is essential for SSE. It tells the browser that the content being sent is an event stream.

2. header('Cache-Control: no-cache'): 

>This directive ensures that the response isn’t cached by the browser, which is important for live data streaming.

## Sending Data:

1. $time = date('r'): 

>This line gets the current server time and formats it according to RFC 2822 (e.g., Mon, 15 Aug 2005 15:52:01 +0000).

2. echo "data: The server time is: {$time}\n\n": 

>This line sends the data to the client. The format data: message\n\n is required for SSE. Each message should be prefixed with data: and suffixed with two newline characters.

## Flushing the Data:

1. flush(): 

>This command is used to flush the output buffer, ensuring that the data is sent to the client immediately. Without flush(), the server might buffer the output, causing delays in data transmission.









