---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "ICS Department Website"
date: 2021
published: true
labels:
  - Java
  - web application design
  - html
summary: "I worked on the ICS page project from Aug2021 untill Aug 2022"
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

I worked on the ICS page project from Aug2021 untill Aug 2022. I took on various tasks from the github repository such as implementing a search bar, testing functions and code. For this project, I was working as a Part time Java Web Developer for the ICS department to help make changes to the ICS website. 

The website was written about 20 years ago, so we had to make some major changes. One of the challenges I took was turining all of the .jsp files into html files while maintaining the functionality and integrity of the .jsp page. This was daunting because some of the .jsp files were well over 500 lines of code. SO I picked piece by piece to try and translate each line and function into html, with fully functioning javascript. 

My first task I implemented a website controler that took on more of the back-end handling of the website such as getting to the proper page, web site functionality and much more. 

For this project, I was the lead programmer who was responsible for programming the various capabilities of the mouse.  I started by programming the basics, such as sensor polling and motor actuation using interrupts.  From there, I then programmed the basic PD controls for the motors of the mouse.  The PD control the drive so that the mouse would stay centered while traversing the maze and keep the mouse driving straight.  I also programmed basic algorithms used to solve the maze such as a right wall hugger and a left wall hugger algorithm.  From there I worked on a flood-fill algorithm to help the mouse track where it is in the maze, and to map the route it takes.  We finished with the fastest mouse who finished the maze within our college.

Here is some code that illustrates how we read values from the line sensors:

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
