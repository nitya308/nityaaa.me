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

The Bootstrap Navbar is organised as follows
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
