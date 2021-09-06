---
theme: default
title: What's New in the World of CSS
class: 'text-center'
highlighter: shiki
lineNumbers: true
download: true
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

---
layout: cover
---

# What We'll Cover?

- #### The Past: CSS History
- #### The Present: Modern CSS
- #### The Future of CSS

---
layout: image-right
image: /grid.png
---

# The Past: CSS History

> Since 1996, We've seen CSS evolve into what we love today, from CSS 1, CSS 2, all the way to CSS 3.

Remember when websites were styled like this? 

Well, a lot has changed over the years. 

### Does the following ring a bell?

- Float and clearfix hack
- Tables
- Support for IE Browsers

<!--
We've even gone from styling layouts with floats and clear, tables for layouts, IE support for styles to more modern layouts like we have today.
-->

---

# The Present: CSS Today

Modern CSS has improved greatly over the years.

We're in a time when it's possible to style layouts with **Flexbox** and **CSS Grid**, and many other possibilites for styling the web.

<figure>
<img src="/word-cloud.png" class="mx-auto" width="600" alt="Word Cloud for CSS Properties">
<figcaption class="text-center text-sm pt-2 text-white underline">
Word Cloud of Some Modern CSS Properties
</figcaption>
</figure>
<!--
Now we're in time where it possible to style your layout with Flexbox and Grid whivh saves us all the headache of styling multi-demensional layout. what else can we do with Modern CSS. I'm pretty sure most of us keep up with the latest in CSS world so some of these might already be familair to you.
-->

---
layout: cover
---

# Modern CSS Features

- Content Visibility
- Scroll Snap
- Aspect Ratio
- Pseudo Class Selectors `:is()`, `:where()`, and `:not()`
- Logical CSS Functions `min()`, `max()`, and `clamp()`
- Container Queries

---

# Content Visibility

Content-visibility enables a user agent to skip an element's rendering work, including layout and painting, until it is needed.

```css
section {
  content-visibility: auto;
}
```
---

## You Should Consider 

- Accessibility Impact
---
layout: center
---

<h1 class="text-center">Demo</h1>

<Codepen width="800" height="400" link="https://codepen.io/lauragift21/embed/RwgGpjZ?default-tab=css%2Cresult&editable=true" />

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

<h1 class="text-center"> Scroll Snap </h1>

Scroll Snap Feature in CSS allows you lock the viewport of certain elements or locations after a user has finished scrolling.

This feature allows you to control panning and scrolling behavior with `snap positions`.

---
layout: center
---

<h1 class="text-center underline">Demo</h1>

<Codepen width="800" height="400" link="https://codepen.io/lauragift21/embed/PojGYVo?default-tab=css%2Cresult&editable=true" />

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

# Aspect Ratio

Aspect ratio is most commonly expressed as two integers and a colon in the dimensions of `width:height`, or `x:y`. 

Maintaining a consistent width-to-height ratio, called an aspect ratio, is critical in responsive web design and helps prevent cumulative layout shift on first load.

<div class="flex justify-center">
  <Codepen width="800" height="300" link="https://codepen.io/lauragift21/embed/jOwMpqB?default-tab=css%2Cresult&editable=true" />
</div>

<!-- Before this feature came to the browser, One way of solving this using the Padding Top Hack.
 This means you need to Calculate the aspect ratio as a percentagee and set it as the padding top property. width:height = height/width * 100 %

Now with the aspect ration property you can directly apply the property to set a defined spect ration for the -->

---
layout: center
---

<h1 class="text-center">Demo</h1>

<Codepen width="800" height="400" link="https://codepen.io/lauragift21/embed/YzQGKmb?default-tab=css%2Cresult&editable=true" />

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
layout: center
class: text-center
---

# Pseudo Class Selectors `:is`, `:where` and `:not()`

---

# `:is()` Selector

The `:is()` pseudo-class function takes a selector list as its argument, and selects any element that can be selected by one of the selectors in that list. This is useful for writing large selectors in a more compact form.

```css
  section > :is(h1, h2, h3, p) {
    font-size: 20px;
  }
```
Translates to the following:

```css
section > h1, section > h2, section > h3, section > p {
  font-size: 20px;
}
```


---

# `:where()` Selector

The `:where()` selector functions the exact way as the `:is()` pseudo-class functions with the exception of a specificity rule applied to it - it's specificity is always zero.

```css{1}
  section > :where(h1, h2, h3, p) {
    font-size: 20px;
  }
```

Translates to:

```css{1}
section > h1, section > h2, section > h3, section > p {
  font-size: 20px;
}
```


---

# `:not()` Selector

The `:not()` pseudo-class represents elements that do not match a list of selectors.

Since it prevents specific items from being selected, it is known as the negation pseudo-class.
```css
  :not(h1, h2, h3, p) {
    font-size: 20px;
  }
```
---
layout: center
---

<h1 class="text-center">Demo</h1>

<Codepen width="800" height="400" link="https://codepen.io/lauragift21/embed/gORwYZY?default-tab=css%2Cresult&editable=true" />

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
layout: center
---

# Logical CSS Functions - `min()`, `max()`, `clamp()`

---
layout: center
---

<h1 class="text-center">Demo</h1>

<Codepen width="800" height="400" link="https://codepen.io/lauragift21/embed/abwmboj?default-tab=css%2Cresult&editable=true" />

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

# Container Queries

Container Queries is one of the newest CSS feature that will allow developers to style `DOM elements` based on the size of a containing element rather than the size of the browser viewport.


<!-- CanIuse Embed -->
<!-- <p class="ciu_embed" data-feature="css-container-queries" data-periods="future_3,future_2,future_1,current,past_1,past_2" data-accessible-colours="false">
<picture class="flex justify-center">
<source type="image/webp" srcset="https://caniuse.bitsofco.de/image/css-container-queries.webp">
<source type="image/png" srcset="https://caniuse.bitsofco.de/image/css-container-queries.png">
<img class="w-3/4" src="https://caniuse.bitsofco.de/image/css-container-queries.jpg" alt="Data on support for the css-container-queries feature across the major browsers from caniuse.com">
</picture>
</p> -->

---
layout: center
---

<h1 class="text-center">Demo</h1>

<Codepen width="800" height="400" link="https://codepen.io/lauragift21/embed/yLXJWGb?default-tab=css%2Cresult&editable=true" />

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
layout: image-right
image: /future.png
---

## What does the future look like?


Expect more improvements and features coming into CSS. This information is based off the snapshot from the CSS Working Group(CSS WG) Current Work.[^1]

These are some of the features you can expect to see coming to CSS in the future:

 - Container Queries - Browser Support.
 - [CSS Nesting Module](https://www.w3.org/TR/css-nesting-1/)
 - CSS Houdini
 - 

 [^1]: [CSS Working Group](https://www.w3.org/Style/CSS/current-work)


---

# Resources

- [A Look Back at the History of CSS](https://css-tricks.com/look-back-history-css/)
- [Selectors Level 4 Draft Spec](https://drafts.csswg.org/selectors-4/)
- [Container Queries](https://css.oddbird.net/rwd/query/)
- [CSS Contain Spec](https://drafts.csswg.org/css-contain/)
- [MDN :is() Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/:is)
- [CSS WG Current Work](https://www.w3.org/Style/CSS/current-work)
- []()
- []()

<!--
I've only scratched the surface in this talk, if you'll love to get into more depth some of the things I shared here today I will recommend you check out the following resources:
-->

---
layout: center
class: text-center
---

# Thank You!

[Slides](https://whatsnewincss.netlify.app/) · [Demos](https://codepen.io/collection/QWjdEv) · [Links](https://linktr.ee/lauragift_)

<p class="text-xs">
  Slides made with 
  <a href="https://sli.dev/" target="_blank">Slidev</a>
</p>
