# Mockups to Code

## Part 2 CSS


### CSS Organization

Each job will have a styleguide on how to organize and style your CSS.

**BONUS**: We can look at an example of a styleguide [at MDN](https://developer.mozilla.org/en-US/docs/MDN/Guidelines/Code_guidelines/CSS)

We can break the current project into

- Build Helpers (delete/comment out at the end)
- General Styles
- Header
- Container
- Aside/Nav
- Main
- Footer

Let's add headers to each section

```CSS
/*********************************
* Build Helpers
*********************************/

/*********************************
* General
*********************************/

/*********************************
* Header
*********************************/

/*********************************
* Container
*********************************/

/*********************************
* Aside/Nav
*********************************/

/*********************************
* Main
*********************************/

/*********************************
* Footer
*********************************/
```


## Header


```CSS
/*********************************
* Header
*********************************/
header {
  width: 90%;
  margin: auto;
  display: flex;
  justify-content: space-between;
  margin-bottom: 20px;
}
```

### Headers Inside of Div

```CSS
header div {
  display: flex;
  flex-wrap: wrap;
  width: 50%;
  margin-bottom: 20px;
}
```

### H1 inside of Header

```CSS
header h1 {
  text-align: left;
}
```

### Last Child of the div inside header

```CSS
header div:last-child {
  display: flex;
  align-items: center;
}
```

###### Appearance

![](./assets/build-progress/header-styled.png)

## Container



```CSS
/*********************************
* Container
*********************************/

.container {
  display: flex;
  width: 90%;
  margin: auto;
  justify-content: space-between;
}

```

###### Appearance

![](./assets/build-progress/container-styled.png)


## Aside/Nav


```CSS

aside {
  flex-basis: 15%;
  min-width: 15%;
  display: flex;
  justify-content: flex-start;
  align-items: center;
}

ul {
  padding: 0;
}

li {
  list-style: none;
  text-align: left;
}
```

## Main

```CSS
/*********************************
* Main
*********************************/

main {
 width: 85%;
 flex-basis: 85%;
}

```


###### Appearance

![](./assets/build-progress/main-styled-1.png)

## Main Rows

```CSS
div[class$='row']  {
   display: flex;
   align-items: center;
   justify-content: space-between;
   margin-bottom: 1em;
 }

.top-row img {
   width: 100%;
}

.middle-row img {
  width: 49%;
}

.bottom-row img {
  width: 32%;
}

```

###### Appearance

![](./assets/build-progress/full-styled-html-w-borders.png)


## Final touches!

Comment out our helper CSS


Full CSS

```css
@import url('https://fonts.googleapis.com/css2?family=Baloo+2&family=Fredoka+One&display=swap');

/*********************************
* Build Helpers
*********************************/

* {
  border: 1px solid mediumvioletred;
}

img {
  width: 100px;
}

/*********************************
* General
*********************************/

body {
  background-color: snow;
  color: slategrey;
  margin: 20px 0;
  font-family: 'Baloo 2', cursive;
  text-align: center;
}

h1, h2, h3, h4, h5, h6 {
  margin: 0;
}

h2 {
  font-size: 1em;
}
h1 {
  font-family: 'Fredoka One', cursive;
}


/*********************************
* Header
*********************************/

header {
  width: 90%;
  margin: auto;
  display: flex;
  justify-content: space-between;
  margin-bottom: 20px;
}

h1 {
  text-align: left;
}

header div:last-child {
  display: flex;
  align-items: center;
}


/*********************************
* Container
*********************************/

.container {
  display: flex;
  width: 90%;
  margin: auto;
  justify-content: space-between;
}

/*********************************
* Aside/Nav
*********************************/

aside {
  flex-basis: 15%;
  min-width: 15%;
  display: flex;
  justify-content: flex-start;
  align-items: center;
}

ul {
  padding: 0;
}

li {
  list-style: none;
  text-align: left;
}
/*********************************
* Main
*********************************/

main {
 width: 85%;
 flex-basis: 85%;
}

div[class$='row']  {
   display: flex;
   align-items: center;
   justify-content: space-between;
   margin-bottom: 1em;
 }

.top-row img {
   width: 100%;
}

.middle-row img {
  width: 49%;
}

.bottom-row img {
  width: 32%;
}

```


## How did we do?
![](./assets/mockups/pillow_talk_full.png)
