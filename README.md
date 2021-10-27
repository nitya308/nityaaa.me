# Nitya's Personal Portfolio

**Author:** Nitya Agarwala  
**Author:** Designed by: Nitya Agarwala  
**Created:** 2021 | **Description:** Nitya's personal portfolio repository.

**Hosted at domain:** https://nityaaa.me

## Basic Details:
**Languages:** HTML, CSS, JavaScript  
**Frameworks:** Bootstrap

## Structure:
The site has 3 main sections:
1. **A Homepage** ```index.html```
2. **About** page ```about.html```
3. **Project** pages describing things I've worked & hobbies ```ldm.html``` ```art.html``` ```match.html```

## Navbar

The Bootstrap Navbar is organised as follows:
 ```
 --navbar
    | -- Projects (dropdown)
    |   |-- Let's Do More (project #1)
    |   |-- Student VolunteerMatch (project #2)
    |   |-- Art(project #3)
    |
    |-- Home
    |
    |-- About
 ```
### Navbar styles
The navbar uses the following bootstrap styles:  
``` <nav class="navbar sticky-top navbar-expand-md navbar-dark bg-dark">``` 
  
```sticky-top```: to keep the position fixed on screen   
```expand-md```: only exppands navbar at > medium devices   
```navbar-dark, bg-dark```: set the black color-scheme for navbar  
  
Following styles are further cutomized from the ```styles.css file```  

```
  .navbar {
  font-size: 1.2em;
  padding-left: 5%;
  padding-right: 5%;
}

.nav-item { 
  margin-left: 10%;
  margin-right: 10%;
}
```  

``` .navbar```  sets padding on the sides of navbar; ``` .nav-item```  ensures sufficient space between each element inside the navbar  

``` 
.nav-link {
  text-align: center;
  text-decoration: none;
}
``` 

``` .nav-link``` aligns all links to the center and overrides the default underline ```text-decoration``` in Bootstrap 

## HomePage

``` index.html```  has the following basic structure  
```
 --index.html
    | -- <section> for introduction
    |   |-- intro text
    |   |-- intro image
    |
    |-- <section> for project #1
    |  |-- <div class = "container"> 
    |    |-- <a href="link to project#1"
    |      |-- heading and tagline
    |      |-- project image
    |
    |-- <section> for project #2
    |  |-- <div class = "container"> 
    |    |-- <a href="link to project#2"
    |      |-- heading and tagline
    |      |-- project image
    |
    |-- <section> for project #3
    |  |-- <div class = "container"> 
    |    |-- <a href="link to project#3"
    |      |-- heading and tagline
    |      |-- project image
 ```  
   
 ### Homepage styles
 Bootstrap containers provide automatic padding and margins for each project card.  
 Each project card also has a unique background color provided to it using the gradient function in ```workstyles.css```.
 
```
#ldm-container{
  background-image: linear-gradient(to bottom right, #BCE9F8, #B8AADC);
}

#match-container{
  background-image: linear-gradient(to bottom right, #FFE9ED, #C9BEE4);
}

#art-container{
  background:linear-gradient(160deg, rgb(217, 255, 147) 0%, rgba(198,240,183,1) 20%, rgba(94,192,187,1) 90%);
}
```

## Project Pages

Each project page follows the same basic template:
```
 --match.html
    | -- <div class = "container"> for **Project Header**
    |   |-- Heading + tagline
    |   |-- 2 responsive header images
    |
    |-- <div class = "container proj-about"> for **About Project**
    |      |-- heading
    |      |-- description + link to the project
    |
    |-- <div class = "row"> for **Project features**
    |      |-- image/text column
    |      |-- image/text column
    |
    |-- <div class = "row"> for more **project features**
    |      |-- image/text column
    |      |-- image/text column
    |
 ```  
 
 ### Project styles  
 Project images have a rounded box and dropshadow along with a caption
 ```  
 .proj-subimg{
  box-shadow: 5px 5px 5px 0px #D3D3D3;
  border-radius: 10px;
}

.img-caption{
  font-size: 0.9em;
  line-height: 1;
  margin: 10px;
}
 ```  
 Gradients are also used to asign each project header a unique color (by ID) for design effect  
 ```  
 #project-art {
  background:linear-gradient(160deg, rgba(255,226,147,1) 0%, rgba(198,240,183,1) 41%, rgba(94,192,187,1) 97%);
}

#project-match {
  background-image: linear-gradient(to bottom, #FFE9ED, #C9BEE4);
}

#project-ldm {
  background-image: linear-gradient(to bottom, #BCE9F8, #B8AADC);
}
 ```  
 
 ## Animated images  
 
 Images on each page are set to **fade in** over 2s using CSS animations in  ```  styles.css ```  
  ```  
 .fade-in-img {
  animation: fadeIn 2s;
  -webkit-animation: fadeIn 2s;
  -moz-animation: fadeIn 2s;
  -o-animation: fadeIn 2s;
  -ms-animation: fadeIn 2s;
}
@keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

@-moz-keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

@-webkit-keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

@-o-keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

@-ms-keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}
  ```  
 ## Buttons
 
 Each page features two buttons at the end: a next button and a previous button. 
 
 ![Image of Yaktocat](https://github.com/nitya308/nityaaa.me/blob/42821aa9fa9c4975db4c81b754980cb58f84c52f/images/buttons.png)
 
 The buttons are styled using a background image for each previous and next button:  
 ```  
 #prev{
  background-image:url("../images/prev.png"); 
  background-repeat: no-repeat;
  background-size: contain;
}

#next{
  background-image:url("../images/next.png");
  background-repeat: no-repeat;
  background-size: contain;
  background-position-x: right;
  background-position-y: bottom;
}
```  

## Hosting  
This website is hosted at: https://nityaaa.me a free domain from Namecheap!
