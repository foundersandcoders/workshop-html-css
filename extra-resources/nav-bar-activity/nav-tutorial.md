# Navbar Tutorial

Follow this tutorial to make a simple navbar. If you get stuck you can have a look at the example in [this directory](https://github.com/foundersandcoders/workshop-html-css/tree/master/nav-bar-activity/nav-example) (but try and work through the tutorial without it as much as you can).

### HTML
First we are going to need to layout our HTML. We are going to make a simple navbar that looks like this:
![Example Wireframe] (https://files.gitter.im/RachBLondon/F70a/Screen-Shot-2016-01-18-at-09.36.23.png)

- create a new folder, and inside that folder create a file called index.html
- create  a basic html outline (Atom will auto complete this for you if you type start to type html and press `enter` (you can use this trick for other html elements as well).
- We are going to use HTML5, so create a `<nav>` tab inside the body (remember to close the tags).


Our Navbar has two main components, the image and the menu tabs.
- create an `<img>` tag, inside you can link to this url  [https://files.gitter.im/RachBLondon/6a6O/logo.png] (https://files.gitter.im/RachBLondon/6a6O/logo.png), or use your own image if you prefer.
- create an `<ul>` tag and fill in the list items as below;
```
      <ul>
        <li>About</li>
        <li>Press</li>
        <li>Contact</li>
        <li>Blog</li>
      </ul>
```

### CSS
If we look at our html layout using a browser, we can see that there are quite a few things we need to change to style the navbar. First lets change the ul elements, we want our menu items to display inline horizontally and with out the default bullet points.
In your *style.css* file, select the *list items in the ul* and apply the following styling.

```
 {
  display: inline;
  padding: 5px;
  text-decoration: none;
}
```
Here we have remove the default styling, and positioned the elements to display in line. I have also added some padding to give a bit of space around each `li` element.

We want our navbar to span the whole page width, so let's set the width to  100%, lets also give it a background colour, and change the font.
```
 nav {
  width: 100%;
  background-color: #FAEBDB;
  font-family:sans-serif;
  }
```

Ok, we still need to position our elements in the navar.


### CSS Flexbox
To position our elements inside the nav we are going to use CSS Flexbox. You can can find a really good guide to [CSS Flexbox here](https://css-tricks.com/snippets/css/a-guide-to-flexbox/).

Flexbox is a great tool to use for positioning which can be difficult in CSS.

To use Flexbox, you need to select a parent element (for this example we will use `nav`). Select `nav` and add the following styling:
`display: flex;` This will make it the container for flexbox.

Great now our navbar is looking alot better, but we still need to move the menu items to the middle of the navbar. This is easy to do with flexbox, add to the parent element (`nav`) the flexbox styling of ` align-items: center;`, great now the image and the text should be both aligned in the middle.

We can use flexbox to move our menu tabs over to the right, again this is easy with flexbox. Just add the follow styling to `nav`, `  justify-content: space-between;`.

### Touching up
Our navbar is now looking pretty good, but you might want to add some right-hand padding to the `ul` element. Select this element and give it ` padding-right:` styling of your choice.

You may also want to give the `ul li` elements a hover over effect. You can do this buy adding:
```
nav ul li:hover {
  color: white;
}
```


Now feel free to change the colour, font or image of your navbar. 

  

