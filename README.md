## Project Summary

In this project, we will be creating a website that will allow us to practice some basic html and css. There is a guided video that you can follow along with to complete this project.

## Goals

- become familiar with common html elements
- add a link that, when clicked, will redirect to another website
- add a link that will sroll to a section on the page
- be able to use ids and classes to target specific elements
- link your css file to your html file
- understand and use semantic html
- understad and use pseudo-class selectors
- understand and use pseudo-element selectors
- understand and use combinator selectors
- understand the box-model
- understand how to add color and images to the backgrounds of elements

## Steps

There are no formal steps in this project.  We are going to recreate the website you see in the image below.  There are many ways we can accomplish this goal.  Follow along with the video if you need guidance, but you can also try to recreate it on your own.  It might be a good idea to do both!

<img width="644" alt="Screen Shot 2020-08-03 at 8 09 05 AM" src="https://user-images.githubusercontent.com/68203064/89191774-a6c92c00-d560-11ea-82fa-8f6bea4a39f7.png">

## Submit project

The final step, and one of the most important! Use git to add and commit any new changes, then push those changes to your reposiroty on github.

Nice work! I hope this was fun for you! You learned a lot in this unit, and your hard work has paid off. Make sure you submit this project in the `Guided project(s)` section for this unit. Just copy the url for your repository, paste it and click send!

## Solution

<details>

<summary>index.html</summary>

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="stylesheet" href="index.css" />
  </head>
  <body>
    <header>
      <h1>Learn</h1>
    </header>
    <section id="banner">
      <h1>This is so cool!</h1>
    </section>
    <section id="content">
      <h1>Learning to code!</h1>
      <p>Click <a href="#schedule">here</a> to see the schedule!</p>
      <p class="aloha-text">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus
        repudiandae itaque ex placeat et delectus dolores eum necessitatibus
        error quae mollitia, eveniet culpa explicabo quibusdam deserunt tempore
        possimus ad obcaecati?
      </p>
      <p class="aloha-text">
        Click <a href="https://google.com" target="_blank">here</a> to go to
        google
      </p>
      <h4 class="who">Who should learn to code?</h4>
      <p>Anyone who...</p>
      <ul>
        <li>wants to learn a new skill</li>
        <li>wants to be relevant</li>
        <li class="next-green">wants to work remotely</li>
        <li>wants extra money</li>
        <li>is looking for a new carrer</li>
      </ul>
      <p>Do any of these apply to you?</p>
      <img
        width="200px"
        src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSxbhCA_yfryp4576uwbMXNK7Kd15sdt9Aggg&usqp=CAU"
      />
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. A incidunt hic
        error nemo praesentium corrupti nihil pariatur repudiandae illum dolore
        aliquam temporibus impedit delectus dolorum sit, sequi, eius ducimus
        itaque.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. A incidunt hic
        error nemo praesentium corrupti nihil pariatur repudiandae illum dolore
        aliquam temporibus impedit delectus dolorum sit, sequi, eius ducimus
        itaque.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. A incidunt hic
        error nemo praesentium corrupti nihil pariatur repudiandae illum dolore
        aliquam temporibus impedit delectus dolorum sit, sequi, eius ducimus
        itaque.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. A incidunt hic
        error nemo praesentium corrupti nihil pariatur repudiandae illum dolore
        aliquam temporibus impedit delectus dolorum sit, sequi, eius ducimus
        itaque.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. A incidunt hic
        error nemo praesentium corrupti nihil pariatur repudiandae illum dolore
        aliquam temporibus impedit delectus dolorum sit, sequi, eius ducimus
        itaque.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. A incidunt hic
        error nemo praesentium corrupti nihil pariatur repudiandae illum dolore
        aliquam temporibus impedit delectus dolorum sit, sequi, eius ducimus
        itaque.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. A incidunt hic
        error nemo praesentium corrupti nihil pariatur repudiandae illum dolore
        aliquam temporibus impedit delectus dolorum sit, sequi, eius ducimus
        itaque.
      </p>
      <div id="schedule">
        <h3>Schedule</h3>
        <div class="scroll-box">
          <ol>
            <li>intro</li>
            <li class="aloha-text last-normal">html/css 1</li>
            <li>html/css 2</li>
            <li>html/css 3</li>
            <li>html/css 4</li>
            <li>html/css 5</li>
            <li>js 1</li>
            <li>js 2</li>
            <li>js 3</li>
            <li>js 4</li>
            <li>js 5</li>
          </ol>
        </div>
      </div>
    </section>
    <section class="box-model-section">
      <p class="left-border">This text has a left border</p>
      <div class="square shadow"></div>
      <div class="large-square shadow large-margin large-padding"></div>
      <div class="half-border square"></div>
    </section>
    <footer></footer>
  </body>
</html>
```

</details>

<details>

<summary>index.css</summary>

```css
* {
  box-sizing: border-box;
}

html,
body {
  padding: 0;
  margin: 0;
  scroll-behavior: smooth;
}

p {
  font-size: 16px;
}

a {
  color: rgb(206, 38, 201);
}

a:hover {
  font-size: 36px;
}

header {
  background-color: black;
  color: greenyellow;
  padding: 8px 48px;
}

#banner {
  height: 500px;
  background-image: url("https://images.unsplash.com/photo-1547394765-185e1e68f34e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2700&q=80");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  text-align: center;
}

#banner > h1 {
  font-size: 48px;
  color: white;
  line-height: 500px;
  margin: 0;
}

#schedule {
  border: 2px dashed green;
  padding: 24px;
  clear: both;
}

#content {
  padding: 48px;
}

.who + p {
  color: rebeccapurple;
}

#content h1 {
  font-size: 64px;
}

.scroll-box {
  border: 1px solid black;
  height: 100px;
  width: 200px;
  overflow: auto;
}

li::selection {
  background: darkred;
  color: honeydew;
}

.aloha-text::after {
  background: greenyellow;
  content: "ALOHA";
}

.last-normal ~ li {
  color: royalblue;
}

.next-green + li {
  color: green;
}

.box-model-section {
  border: 3px solid red;
  margin: 8px;
  padding: 24px;
}

.left-border {
  border-left: 2px solid black;
}

.square {
  height: 100px;
  width: 100px;
}

.half-border {
  border-left: 2px solid black;
  border-bottom: 2px solid black;
}

.large-margin {
  margin: 28px;
}

.large-padding {
  padding: 28px;
}

.large-square {
  height: 200px;
  width: 200px;
}

.shadow {
  box-shadow: 4px 4px 13px 0px rgba(21, 19, 19, 0.4);
}

img {
  float: left;
  margin-right: 16px;
  margin-bottom: 16px;
}
```

</details>
