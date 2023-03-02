# CSS Tutorial Project

This repo is an intro project to basic CSS styling.<br/>
It will have inline, internal and external css styling.
<br/>
<br/>

### Inline CSS
We can use the style attribute within the tags to add styling by selecting the keyword: value ;
<br/>
While it is easy to make changes on the fly. There is a downside. If you have a lot of similar elements that you would like to change, then you would need to make changes to each of them individually. I also make your html code harder to read.
<br/>
<br/>

### Internal CSS
One way to use internal css is to add the style element within the head tag and add the keyword:values for the elements we want to change. We do this by selecting the tag we want to change and then inside the curly braces adding all the keyword:value; pairs we want to use.
<br />
* example: h1{ color: red; font-size:50px;}
<br/>
All the changes you make in the head section cascade to all the same tag elements on the same page.
<br/>
This works great, but when you have more than 1 page website, you will need to add the same styling inside the head tag, and if you ever need to make changes, you will need to go into each page and update all the styling. This is also a bit ineffecient.
<br/>
<br/>

### External CSS
This is a better solution to cascade changes throughout all the pages and their elements to keep the site cohesive. 
<br/>
To do this, create a folder called css and inside the folder create a file called styles.css. This file will hold all the css code for the website.
<br/>

* example: link rel="stylesheet" href="./css/styles.css"
<br/>
<br/>

### Power Struggle
There is a challenge when using all the external, internal and inline styling. 
<br/>
The first style is from the external sheet, that can be overwritten by internal styles for the properties that are being changed. The inline style overwrites the properties of both the External and Interal styling. 
<br/>
This is called the Last-Rule. What ever is last changed is the styling that takes place.
<br/>
<br/>

### Basic Syntax
Syntax is composed of the selector, the opening and closing curly braces, and the property:value pairs.<br/>
Altogher,these are called CSS rules
* rule example: h1 { color: red;}
<br/>

The h1 is the selector, and everything inside the curly braces are the declarations to apply to that element tag
<br>
We can target more than just tags, we can apply styling to classes, and ids
<br/>
<br/>

### Grouping Selectors
We can group selectors that we want to have the same CSS rules by naming the selector adding a comma and then adding the next selector <br/>

* example :  h1,p, #name (ID), .section (class)

<br/>
<br/>

### ID Selectors
In order to target an element tag by its ID, we have to add an id="name" to the element inside our html code, and then use the hasthag with the name of the id we want to select and add css rules to.

* example: #footer { color: orange}

<br/>
Please note that any declaration within the id will be applied only to that element tag with the unique id. 
<br/>
<br/>

### Class Selectors
If we want different elements to have the same styling we can add the class name attribute inside the element tag and then in CSS use the dot preceeding the name as the selector.
<br/>

* example: class="sectionbox" inside the element tag
* example: .sectionbox { background-color: lightgrey;} in the css

<br/>
<br/>

### Inheritence
Inheritence basically means that any element tags inside another element tag will inherit the parent styling unless that element has it's own styling.
<br/>
<br/>

### Specificty
In CSS the more specific the selector then that particular style will be applied. The order of specificty is as follows:
<br/>

* ID - most specific
* Class - next specific
* Element - least specific

<br/>
<br/>
To learn more about specificity visit:
<br/>

[CSS Specificty](https://www.w3schools.com/css/css_specificity.asp) 