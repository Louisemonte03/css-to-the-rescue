# css-rescue louise

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
- **Wat ga ik morgen doen**
  Tomorrow I’ll start deciding which CSS elements I’m going to use in the code.

Code elements I’ll use:
HTML

- A div or canvas for the play area
- A div for the duck

CSS

- position: absolute on the duck so it can move
- border-radius for round shapes like body and head
- transform for rotation beak, tail
- transition for smooth movement
  animation + @keyframes for a waddle animation

## **Dag 2 dinsdag**

- **Wat heb ik gedaan?**

I started working on creating the duck and the two themed backgrounds.

The duck →-

- The duck for me was a little difficult. I want to ask Sanne or Nils for help on this one
  ![the duck i now got](/images/readme/the-duck.png)

The background themes →

- For the background themes, I worked on making a scene with clouds, bushes, and water. At first the clouds didn’t work properly, because when the screen became smaller everything shifted. I eventually fixed this by using percentages instead of fixed values.

I used radio buttons together with display: none and display: block so that when you select the “in water” option, the water background appears.

I implemented this with radio buttons. It’s the same technique I learned in Browser Tech to hide certain content and show it when something is selected.
![theme switcher with radio buttons](/images/readme/theme-switcher-code.png)
![what i now got](/images/readme/what-i-now-got.png)

- **Hoe lang duurde het ?** The whole day
- **Wat heb ik geleerd?** I Learned how to adjust the sizes with postion absolute on % so that my illustrations dont move. And also how to work without using classses and id's

- **Wat ga ik volgende week doen** Next week i want to start with the duck. Then im gonna focus on the movment.

## Week 2 — De eend bouwen & animaties

- **Wat heb ik gedaan?**

This week I focused on building the duck entirely out of css and htmm. The duck is made up of basic html elements div for the head and body, span for the eye, button for the beak, article for the wing, aside for the tail connector, and ul li for the legs and feet.

I added css animations for the walking motion. The legs swing back and forth using keyframes legwing with transform: rotate. The body has a gentle bounce with keyframes hop body. The wing flaps using steps to give it a more cartoon movement.

I also structured the css using layer theme, base, duck, interaction, animation so everything stays organized and easy to adjust.

- **Wat was moeilijk?**
  Getting the legs to look right took a lot of trial and error. The transform origin had to be set to top center so the legs swing from the hip rather than the center. Also figuring out the right nth-of-type selectors without using classes was a challenge but also very satisfying once it worked.

- **Wat heb ik geleerd?**

I learned how to structure CSS with layer and how powerful CSS nesting is for keeping code readable. I also got more comfortable with keyframes and animation timing.

## Week 3 — Road Runner & omgeving

- **Wat heb ik gedaan?**

This week I added the full background scene and the Road Runner interaction. The background has:

- A sky gradient
- Animated clouds drifting from right to left
- A ground with a grass strip on top
- A CSS tree
- A water mode with oval ripple animations

For the Road Runner mode checkbox toggle, the duck gets a spinning fire ring underneath it — built with conic-gradient and a mask to create the ring shape. In Road Runner mode, everything speeds up: clouds, the tree, and the duck itself runs across the screen using translateX.

I added a water and Road Runner combo where the duck tilts like a speedboat rotate-20deg and shoots across the screen.

- **Wat was moeilijk?**
  Getting the CSS only interaction to work correctly was the hardest part. Since I can't use javascript, everything has to work with :checked sibling selectors. Combining multiple states land/water + silly in one selector was confusing at first. Also understanding why the selector only works in a specific dom order took some time.

- **Wat heb ik geleerd?**
  I learned a lot about css animations and how animation duration can be overridden in a more specific selector to speed things up. I also learned how conic-gradient and mask work together to create a ring shape. And I deepened my understanding of the CSS cascade and how layer controls priority.

## Week 4 — Afronding & refactoring

- **Wat heb ik gedaan?**

In the final week I did a big refactor: I removed all classes from the html and css. The assignment says to work without classes except one if strictly necessary, so I replaced everything with structural selectors.

I also cleaned up the CSS and made sure all interactions still worked correctly after the refactor.

Final result overview:

- Land mode: duck walks with animated legs, tree drifts by, clouds float
- Water mode: duck floats and bobs, ripples animate in the water
- Road Runner: duck sprints across the screen, everything speeds up, fire ring appears
- Water + Road Runner: duck tilts and shoots across the water like a speedboat

- **Wat ging goed?**

The overall concept came together nicely. The combination of @layer, CSS nesting, :checked selectors and keyframes creates a lot of interaction with zero JavaScript.

- **Wat was uitdagend?**

Removing all classes and replacing them with nth-of-type selectors was tedious but taught me a lot about how CSS selectors really work. It also made me realise how important good HTML structure is.

- **Wat wil ik nog verder verkennen?**

I'd like to explore CSS container queries and property for animating custom properties. Also scroll-driven animations look interesting for future projects.

## Bronnen

### CSS technieken

- [MDN — CSS @layer](https://developer.mozilla.org/en-US/docs/Web/CSS/@layer)
- [MDN — CSS Nesting](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_nesting)
- [MDN — CSS Animations / @keyframes](https://developer.mozilla.org/en-US/docs/Web/CSS/@keyframes)
- [MDN — conic-gradient()](https://developer.mozilla.org/en-US/docs/Web/CSS/gradient/conic-gradient)
- [MDN — mask](https://developer.mozilla.org/en-US/docs/Web/CSS/mask)
- [MDN — :checked selector](https://developer.mozilla.org/en-US/docs/Web/CSS/:checked)
- [MDN — :nth-of-type()](https://developer.mozilla.org/en-US/docs/Web/CSS/:nth-of-type)
- [MDN — transform](https://developer.mozilla.org/en-US/docs/Web/CSS/transform)
- [MDN — clip-path](https://developer.mozilla.org/en-US/docs/Web/CSS/clip-path)

### AI

- Claude (Anthropic) — gebruikt om code op te schonen en te structureren
