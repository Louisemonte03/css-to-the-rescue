# css-rescue

## **Project Overview**

Your task: Create an interactive CSS-only silly walk (or
an interactive instruction for performing a silly walk).

## **Technische Specificaties**

## **Dag 1 maandag**

- **Wat heb ik gedaan?**Today I worked on coming up with a concept. After thinking it through, I decided to go with the silly walk assignment. I brainstormed a few ideas and chose to make a duck. The duck won’t be an SVG; I’m going to build it with CSS.

The idea is a duck that walks, but I’m still figuring out what kind of silly walk it will have. First I need to design the duck and gather some inspiration. The duck will move with the arrow keys, eat with the space bar, and speed up when doing so.

I also created some mood boards with matching colors to get a sense of the atmosphere I want to create. I’m going to make a duck that can either swim or walk; those are the two themes I’ll be working with.

I’ve already added the colors I want to use for the duck and the background themes to my stylesheet.
![visual idea](/images/readme/visualisation-idea.png)
![the colors i choose for the customproperties](/images/readme/colors-root.png)
![moodmoard](/images/readme/moodboard-visual.png)

- **Hoe lang duurde het ?** The whole day
- **Wat heb ik geleerd?** ///
- **Wat ga ik morgen doen**

Tomorrow I’ll start deciding which CSS elements I’m going to use in the code.
Code elements I’ll use

HTML
A div or canvas for the play area
A div for the duck (or multiple divs for body, head, beak, tail)
Optional span elements for details

CSS
position: absolute on the duck so it can move
border-radius for round shapes (body, head)
transform for rotation (beak, tail)
transition for smooth movement
Pseudo-elements ::before and ::after for extra shapes without extra HTML
animation + @keyframes for a waddle animation with slight rotation and animation delay

## **Dag 2 dinsdag**

- **Wat heb ik gedaan?**

I started working on creating the duck and the two themed backgrounds.

The duck →
The duck for me was a little difficult. I want to ask Sanne or Nils for help on this one
![the duck i now got](/images/readme/the-duck.png)

The background themes →
For the background themes, I worked on making a scene with clouds, bushes, and water. At first the clouds didn’t work properly, because when the screen became smaller everything shifted. I eventually fixed this by using percentages instead of fixed values.

I used radio buttons together with display: none and display: block so that when you select the “in water” option, the water background appears.

I implemented this with radio buttons. It’s the same technique I learned in Browser Tech to hide certain content and show it when something is selected.
![theme switcher with radio buttons](/images/readme/theme-switcher-code.png)
![what i now got](/images/readme/what-i-now-got.png)

- **Hoe lang duurde het ?** The whole day
- **Wat heb ik geleerd?** I Learned how to adjust the sizes with postion absolute on % so that my illustrations dont move. And also how to work without using classses and id's

- **Wat ga ik volgende week doen** Next week i want to start with the duck. Then im gonna focus on the movment.
