---
theme: default
title: What's New in the World of CSS
# like them? see https://unsplash.com/collections/94734566/slidev
# background: https://source.unsplash.com/collection/94734566/1920x1080
class: 'text-center'
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## What's New in the World of CSS & The Future of CSS
  Presentation by Gift Egwuenu.
  Frontend Developer Consultant at [Passionate People](https://passionatepeople.io)
---

# What's New in the World of CSS

& The Future of CSS

Infobip Shift Dev 2021

[@lauragift_](https://twitter.com/lauragift_)

<div class="abs-br m-6 flex gap-2 pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    <carbon:arrow-right class="inline text-4xl"/>
  </span>
</div>

<!-- 

The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

--- 
layout: cover
class: text-left
---
# Who Am I?

## Gift Egwuenu 

Frontend Developer Consultant at [Passionate People](https://passionatepeople.io) <br> and Content Creator based in the Netherlands.


[@lauragift_](https://twitter.com/lauragift_)

[giftegwuenu.com](https://giftegwuenu.com)

<div class="flex">
<img class="rounded-1/2 h-60 abs-tr mt-36 mr-16" src="https://res.cloudinary.com/lauragift/image/upload/v1624353138/4EFA5623-1143-4480-A319-F5389240D87A_hgsluf.jpg" alt="Gift Egwuenu">
</div>


<div class="abs-br m-6 flex gap-2 pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    <carbon:arrow-right class="inline text-4xl"/>
  </span>
</div>

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent; 
  -moz-text-fill-color: transparent;
}
</style>

---

# What We'll Cover?

In this talk, I will cover the different eras in CSS History.

- ### The Past: CSS History

- ### The Present and
- ### The Future of CSS

<!-- https://sli.dev/guide/animations.html#click-animations -->
<!-- <img
  v-click
  class="absolute -bottom-9 -left-7 w-80 opacity-50"
  src="https://sli.dev/assets/arrow-bottom-left.svg"
/>
<p v-after class="absolute bottom-23 left-45 opacity-30 transform -rotate-10">Here!</p> -->

---
layout: image-right
image: https://res.cloudinary.com/lauragift/image/upload/v1630866765/Grid_cam1d9.png
---

# The Past: CSS History

> Since 1996, We've seen CSS evolve into what we have today, from CSS 1, CSS 2, and CSS 3.

Remember when websites were styled like this? 

Well, a lot has changed over the years.

We've even gone from styling layouts with Floats for positioning, IE Support for Styles and Tableessss to more modern layout and styles like we have to today.

<arrow v-click="3" x1="400" y1="420" x2="230" y2="330" color="#564" width="3" arrowSize="1" />

[^1]: [Image Credits](https://css-tricks.com/look-back-history-css/)

<style>
.footnotes-sep {
  @apply mt-20 opacity-10;
}
.footnotes {
  @apply text-sm opacity-75;
}
.footnote-backref {
  display: none;
}
</style>

---

# The Present: CSS Today

Modern CSS is 

We're in a time where it's possible to style layouts with Flexbox and Grid. 


<!-- Now we're in time where it possible to style your layout with Flexbox and Grid whivh saves us all the headache of styling multi-demensional layout. what else can we do with Modern CSS. I'm pretty sure most of us keep up with the latest in CSS world so some of these might already be familair to you. -->
---
layout: center
class: px-20
---

# What does the Future look like?

Slidev comes with powerful theming support. Themes can provide styles, layouts, components, or even configurations for tools. Switching between themes by just **one edit** in your frontmatter:

Read more about [How to use a theme](https://sli.dev/themes/use.html) and
check out the [Awesome Themes Gallery](https://sli.dev/themes/gallery.html).

---

# Resources

- [A Look Back at the History of CSS](https://css-tricks.com/look-back-history-css/)
- 
- 
- 
<!-- I've only scratched the surface in this talk, if you'll love to get into more depth some of the things I shared here today I will recommend you check out the following resources: -->
---
layout: center
class: text-center
---

# Thank You!

[Slides](https://sli.dev) · [Demos](https://github.com/slidevjs/slidev)

<p class="text-xs">
  Slides made with 
  <a href="https://sli.dev/" target="_blank">Slidev</a>
</p>
