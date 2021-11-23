# Learning-JavaScript
These are the notes I wrote down while learning about JavaScript through "TheOdinProject" course, and many other resources! <br>
# DOM manipulation 
<b>DOM - Document object model</b> <br>
The DOM (or Document Object Model) is a tree-like representation of the contents of a webpage - a tree of “nodes” with different relationships depending on how they’re arranged in the HTML document. <br>
<br>
<b>Targeting nodes with selectors</b> <br>
When working with the DOM, you use “selectors” to target the nodes you want to work with. You can use a combination of CSS-style selectors and relationship properties to target the nodes you want. <br>
<br>
<b>DOM methods</b> <br>
When the HTML code is parsed by a web browser, it is converted to the DOM.<br>
<u>Query selectors:</u> <br>
⚫ element.querySelector(selector) returns reference to the first match of selector<br>
⚫ element.querySelectorAll(selectors) returns a “nodelist” containing references to all of the matches of the selectors<br>
<br>
It’s important to note that when using querySelectorAll, the return value is not an array. It looks like an array, and it somewhat acts like an array, but it’s really a “nodelist”. The big distinction is that several array methods are missing from nodelists. <br>
<br>
<b>Element creation</b><br>
⚫document.createElement(tagName, [options]) creates a new element of tag type tagName. [options] in this case means you can add some optional parameters to the function.<br>
<br>
const div = document.createElement('div'); <br>
This function does NOT put your new element into the DOM - it simply creates it in memory. This is so that you can manipulate the element (by adding styles, classes, ids, text etc.) before placing it on the page. You can place the element into the DOM with one of the following methods.<br>
<br>
<b>Append elements</b><br>
⚫parentNode.appendChild(childNode) appends childNode as the last child of parentNode<br>
⚫parentNode.insertBefore(newNode, referenceNode) inserts newNode into parentNode before referenceNode<br>
<br>
<b>Remove elements</b><br>
<br>
⚫parentNode.removeChild(child) removes child from parentNode on the DOM and returns reference to child<br>
<br>
<b>Altering elements</b><br>
<br>
When you have a reference to an element, you can use that reference to alter the element’s own properties. This allows you to do many useful alterations, like adding/removing and altering attributes, changing classes, adding inline style information and more.<br>
