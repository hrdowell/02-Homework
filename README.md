# 02-Homework: Advanced CSS Portfolio🎨

#### For this assignment, I created a portfolio for myself from scratch, using advanced CSS properties like flex, grid, and responsive layout. 
- Here is a link🔗 to the final deployed application, "Hannah Dowell's Portfolio":
https://hrdowell.github.io/02-Homework/.


### Assignment Details

### User Story

```
AS AN employer
I WANT to view a potential employee's deployed portfolio of work samples
SO THAT I can review samples of their work and assess whether they're a good candidate for an open position
```

## Acceptance Criteria

Here are the critical requirements necessary to develop a portfolio that satisfies a typical hiring manager’s needs:

```English
GIVEN I need to sample a potential employee's previous work
WHEN I load their portfolio
THEN I am presented with the developer's name, a recent photo or avatar, and links to sections about them, their work, and how to contact them
WHEN I click one of the links in the navigation
THEN the UI scrolls to the corresponding section
WHEN I click on the link to the section about their work
THEN the UI scrolls to a section with titled images of the developer's applications
WHEN I am presented with the developer's first application
THEN that application's image should be larger in size than the others
WHEN I click on the images of the applications
THEN I am taken to that deployed application
WHEN I resize the page or view the site on various screens and devices
THEN I am presented with a responsive layout that adapts to my viewport
```



## 🎯Getting started with a wireframe

To stay organized while creating an application with multiple advanced CSS properties, I knew I wanted to get started with wireframing🖼. I listed all of the requirements for my website and sketched out a UI that incorporated all of them:

<img src="assets\02-homework@2.5x.png" style="zoom:33%;" />

I decided that the WORK section CSS would include the measurement "rem" and CSS properties like ""<width: 100%;" & "font-size: 3em;" to ensure that it is responsive on any device. I knew I wanted to use responsive measurements so that the transitions from one size to another on the UI was not choppy or messy. This way, users can view a clean and evenly-proportioned website no matter the screen size.



## 🎯Formatting the HTML file

- I seamlessly created my index.html file based on the wireframe I had just created. 
- I was sure to create a header with a nav section that lists about, work, and contact with relative links to the sections with corresponding id's. 

<img src="assets\02hwcommit1nav.PNG" style="zoom:33%;" />

- I created div's with the id "about" and "work", with semantic tags between them for the "work" section. Because I knew I would be styling 5 images in a grid layout, I kept the heading element "h2 id= 'work'" element outside of the section that would get a grid layout. I included figure tags with figcaption tags nested inside, all inside of a section tag that I would later format using grid. I gave the first box a unique id, "box1" because it needed to be larger than the other images. 
- With all images uploaded, I included alt tags to make my website accessible to those with disabilities. 💡I also included "target='_blank'" within the "a" tags for each image and contact links, so that the linked websites would open in a new tag.💡 

<img src="assets\02hwcommit1section.PNG" style="zoom:33%;" />

- I created a Contact div within the main tags and finished up the index with a footer, containing a paragraph.

## 🎯Creating a responsive stylesheet

- I uploaded a google fonts stylesheet with the fonts Tenor Sans for headings and Montserrat for body text. 
- Next, I created sections within the CSS using comments for the header, main, "My Work" section, and the footer
- For the header, I knew I could use flex💪 styling with responsive measurements (em, rem). I used "justify-content: space-between" to evenly space out my headshot image, title (Hannah Dowell) and navigation links across the header. I used flex-direction: column, justify-content: center to align the nav links to match my wireframe🖼. Then, I added the pseudo class "nav a:hover" to add a box around each nav link only when hovered over. The first step ensures that the header is responsive and the second that it is dynamic and interesting.

<img src="assets\02hwcommit2cssnav.PNG" style="zoom:33%;" />

- Next, I styled the div & h2 elements using the percentage and rem units so that the page would be responsive.
- I styled the section element to create a grid that contains all of the figures, which contain links to my applications. 💡I used the newer element **"fr"** unit to help make the grid responsive. 💡
- I used the pseudo class ":hover"🛸 to change the opacity of the figures when the mouse hovers over them. I also added the property "max-width: 100%" to all image elements so that they will change sizes proportionate to the size of the screen.
- Lastly, I added a media query at the end of my CSS file to modify my application for smaller screens. I decreased font size and margins across the board. I changed the grid layout for the "my work" section to a simpler inline-block style, while maintaining that the first figure appeared larger than the rest. These changes apply to screens that are 768px wide and smaller.


<img src="assets\02hwcommit2csswork.PNG" style="zoom:20%;" />

## 🎯The final product

<img src="assets\02hwscreenshot.PNG" style="zoom:30%;" />

- Here is a link🔗 to the final deployed application, "Hannah Dowell's Portfolio":
https://hrdowell.github.io/02-Homework/.