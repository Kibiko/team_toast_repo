# BNTA - Shop landing page assessment day solution

This is a solution to the Shop landing page BNTA assessment day which allows us to show off some of the HTML, CSS and JavaScript we've learnt.

## Table of contents

- [Overview](#overview)
  - [Our users should be able to](#our-users-should-be-able-to)
  - [Stretch Goals](#stretch-goals)
- [The process](#The-process)
  - [Built with](#built-with)
  - [What I learned](#what-we've-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#authors)
- [Acknowledgments](#acknowledgments)

### Overview

The project was to design and build a simple website using HTML and CSS techniques learnt during the assessment day. We also got to chose the theme of our website and we decided to with a bakery!

### Our users should be able to:

-The user should be able to browse and buy a selection of tasty pastries, cakes and cookies. 
-The user should be able to navigate to their preffered choice of snack using the header, footer or links throughout the page.


### Stretch goals:

- Implement a Dark Mode button using HTML and JavaScript. The the user should be able to enable dark mode to use the website when they require a midnight snack.

## The process

Initially we had to come up with a team name, decide on a topic, work out what tasks needed to be completed and then assign those tasks to the group members. We chose to use Trello to manage this.
Step two was to design the web page. We used iDroo to scribble down a sketch of what we wanted the website to look like and what content it should contain.
Next we started to write the HTML and CSS for the website, ironing out bugs along the way with help from all the group members.
Finally we went through the webpage top to bottom adding any finishing touches to area's that team members highlighted as being in need of a little polish.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- JavaScript

### What we've learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge and will also serve to guide you through preparing for your presentation.

To see how you can add code snippets, see below:

Rohaib:

```html
<div class ="column">
                        <img class="categories1" src = "https://images.unsplash.com/photo-1576618148332-a18871379090?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=449&q=80"/>
                        <h2>Carrot Cake</h2>    
                        <h3 class = "Rohaib">£1000</h3> 
                        <button class ="center1" type="button" onclick="alert('Added to Basket')">Add to Basket!</button>
                    </div>
```
                    
I learnt that you can directly import images from the internet onto your html code, this made the process very efficient otherwise we'd all have had to save over 10 images onto our computers and import them manually onto our website. 


Kevin:

Separating the width of the page into three columns with floating pictures side by side. I have learnt to make sure to clear the content after the last element of the float in case other floating elements from different sections tried to sneak onto the side of the three category pictures.

```html
<div class="row">
                <div class="column">
                    <a href="#Pastries"><img class="categories" alt="Pastries" title="Pastries" src="https://images.unsplash.com/photo-1483695028939-5bb13f8648b0?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80"/></a>
                    <h2 id="cat_title">Pastries</h2>
                </div>
                <div class="column">
                    <a href="#Cakes"><img class="categories" alt="Cakes" title="Cakes" src="https://images.unsplash.com/photo-1622896784083-cc051313dbab?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8NXx8Y2FrZXN8ZW58MHx8MHx8fDI%3D&auto=format&fit=crop&w=400&q=60"/></a>
                    <h2 id="cat_title">Cakes</h2>
                </div>
                <div class="column">
                    <a href="#Cookies"><img class="categories" alt="Cookies" title="Cookies" src="https://images.unsplash.com/photo-1634188023730-2a607e9c27a2?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8NTd8fGNvb2tpZXN8ZW58MHx8MHx8fDI%3D&auto=format&fit=crop&w=400&q=60"/></a>
                    <h2 id="cat_title">Cookies</h2>
                </div>
            </div>
```
```css
.row::after{
    content: "";
    clear: both;
    display: block;
}
```

Dominic:

I'm really proud of the header bar which has a combination of links and button's that have been formatted to look the same. As weel as when a user hover's over an option from the menu bar it highlights the box.

```HTML
<header id="Header">
        <!-- This is where the header will go -->
        <ul>
            <li></li>
            <li><a href="index.html">Home</a></li>
            <li><a href="#About">About</a></li>
            <li><a href="#Footer">Contact</a></li>
            <li><button onclick="myFunction()">Dark Mode</button></li>
        </ul>
    </header>
```
```css
li a, li button {
    display: block;
    color: #8b6731;
    padding: 1em 1em;
    text-align: center;
    text-decoration: none;
    font-size: 180%;
}

li a:hover, li button:hover {
    background-color: #f5d5a9;
    text-decoration: underline;
}

li button:hover {
    cursor: pointer;
}
```

Faran:

I used the flexbox to centre out the "Click to Buy!" button. Since all other display functions were not providing the required result, I tried using the flex display, which helped to centre the buttons and look as required.

```css
.center1 {
    display: flex; 
    justify-content: center;
    align-items: center;
    margin: auto;   
}
```
I also added a picture and text side to side. I learnt to format the pieces so they fit together on the page, without any overlaps or large spaces.

### Continued development

For future projects it would be helpful to be able to change all components of the website to dark-mode when the dark-mode is used by the user. Currently, we can change most of the webiste to dark-mode but the backgorund color of the header and footer remain the same.

Also, we can adapt the website to be accessible to a larger user base, which would include mobile phones, tablets or consoles.



### Useful resources

- [W3Schools](https://www.w3schools.com/) - This is so helpful for checking HTML, CSS and JavaScript syntax or learning about different properties and containers.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Authors

- Team Toast Bakery! - [Dominic Romana, Kevin Chan, Muhammad Faran Sarwar, Rohaib Ahmed]

## Acknowledgments

We would like to say a quick thank you to whoever created the doritos website because that made us all hungry which then inspired us to choose a bakery theme. 
We would also like to thank the creators of Eporium Pies website since the colour them took inspiration from their websites colour pallet. (https://dt2sdf0db8zob.cloudfront.net/wp-content/uploads/2019/03/20-Inspiring-Bakery-Websites-image10.jpg)
Lastly a quick thanks to Phil, Colin, Ed and all the consultant's at Bright Network. Without your guidance thise project wouldn't have been possible.
