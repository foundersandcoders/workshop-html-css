#Navbar Tutorial

Follow this tutorial to make a simple Navbar.

###HTML
First we are going to need to layout our HTML. We are going to make a simple navbar that looks like this:
![Example Wireframe] (https://files.gitter.im/RachBLondon/F70a/Screen-Shot-2016-01-18-at-09.36.23.png)

- create a new folder, and inside that folder create a file called index.html
- create  a basic html outline (Atom will auto complete thisi for you if you type start to type html and press `enter` (you can use this trick for other html elements as well).
- We are going to use HTML5, so create a `<nav>` tab inside the body (remember to close the tags).

Our Navbar has two main components, the image and the menu tabs.
- create an `<img>` tag, inside you can link to this url https://files.gitter.im/RachBLondon/2jvS/logo-01.png  (you wont see the logo yet as it white).
- create an `<ul>` tag and fill in the list items as below;
```
      <ul>
        <li>About</li>
        <li>Press</li>
        <li>Contact</li>
        <li>Blog</li>
      </ul>
```


####CSS 
- Now, in the same folder create a file called style.css
- Link your CSS file in the head of your index.html file
  `    <link rel="stylesheet" href="style.css" media="screen" title="no title" charset="utf-8">`
- Lets give the whole nave element a background colour and a height
```
nav {
  background-color: #e3e0cf;
  height: 6em;
}
```
- Now we want to change our menu items to diplay inline and take away the ugly bullet points, lets also change the font. To do this, select the `li`, inside the `ul` and add the following css.
```
{
  display: inline;
  text-decoration: none;
  font-family: sans-serif;
}
```
- The menu items now diplay in row, but they are outside the navbar. This is because the `ul` element is set to `display : block` by default. Let's get rid of this by adding the following CSS to the UL elements:
```
{
  display: inline;
}
```
  

