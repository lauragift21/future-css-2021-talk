---
theme: default
title: What's New in the World of CSS
# background: https://images.unsplash.com/photo-1621839673705-6617adf9e890?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=3589&q=80
class: 'text-center'
highlighter: shiki
lineNumbers: false
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


### Does the following ring a bell?

- Float and Clearfix Hack
- Tables
- Support for IE Browsers

Well, a lot has changed over the years...

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
Word cloud of some modern CSS properties
</figcaption>
</figure>

<!--
Now we're in time where it possible to style your layout with Flexbox and Grid whivh saves us all the headache of styling multi-demensional layout. what else can we do with Modern CSS. I'm pretty sure most of us keep up with the latest in CSS world so some of these might already be familair to you.
-->

---
layout: cover
---

# Modern CSS Features

- Scroll Snap
- Aspect Ratio
- Pseudo Class Selectors `:is()`, `:where()`, and `:not()`
- CSS Math Functions `min()`, `max()`, and `clamp()`
- Container Queries

---
layout: cover
---

# Scroll Snap

The Scroll Snap feature in CSS introduces scroll `snap positions`, which enforce the scroll positions that a scroll container’s scrollport may end at after a scrolling operation has completed.

```css
.parent {
  scroll-snap-type: x mandatory;
}

.child {
  scroll-type-align: start;
}
```

---
layout: center
---

<figure class="mx-auto text-center">
<img class="mx-auto w-3/4" src="https://caniuse.bitsofco.de/static/v1/css-snappoints-1630926323687.png" alt="Data on support for the css-snappoints feature across the major browsers from caniuse.com">
<figcaption class="pt-4 underline">
  Browsers Support - Data from caniuse.com
</figcaption>
</figure>

---
layout: center
---

<h1 class="text-center text-4xl">Demo</h1>

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

<!-- Here's how it works. You need to set the scroll-type property to a parent container with values being either x mandatory or y mandatory. and the child container will also need to set a scroll-align-type property of which the values here can be `start`, `center`, `end`. -->
---

# Aspect Ratio

Aspect Ratio is most commonly expressed as two integers and a colon in the dimensions of `width:height` or `x:y`. This can be applied to images or video elements. i.e 16:9, 4:3 aspect ratio.

### Solutions for Aspect Ratio

<br>

Padding-Top Hack

```css
img {
  width: 100%;
  padding-top: 56.6%; /* 16:9 Aspect Ratio Calculated as 9 / 16 * 100 */
}
```

Native support for Aspect Ratio

```css
img {
  width: 100%;
  aspect-ratio: 16 / 9;
}
```

<!-- Before this feature came to the browser, One way of solving this using the Padding Top Hack.
 This means you need to Calculate the aspect ratio as a percentagee and set it as the padding top property. width:height = height/width * 100 %

Now with the aspect ration property you can directly apply the property to set a defined spect ration for the -->

---
layout: center
---

<figure class="mx-auto text-center">
<img class="mx-auto w-3/4" src="https://caniuse.bitsofco.de/static/v1/mdn-css__properties__aspect-ratio-1630926408118.png" alt="Data on support for the css-snappoints feature across the major browsers from caniuse.com">
<figcaption class="pt-4 underline">
  Browsers Support - Data from caniuse.com
</figcaption>
</figure>


---
layout: center
---

<h1 class="text-center text-4xl">Demo</h1>

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
layout: center
---
# `:is()` Selector

The `:is()` pseudo-class function takes a selector list as its argument, and selects any element that can be selected by one of the selectors in that list. This is useful for writing large selectors in a more compact form.

```css
  section > :is(h1, h2, h3, p) {
    font-size: 20px;
  }
```

Translates to:


```css
section > h1, section > h2, section > h3, section > p {
  font-size: 20px;
}
```

---
layout: center
---

# `:where()` Selector

The `:where()` selector functions the exact way as the `:is()` pseudo-class functions with the exception of a specificity rule applied to it - it's specificity is always zero.

```css
  section > :where(h1, h2, h3, p) {
    font-size: 20px;
  }
```

Translates to:

```css
section > h1, section > h2, section > h3, section > p {
  font-size: 20px;
}
```

---
layout: center
---

# `:not()` Selector

The `:not()` pseudo-class represents elements that do not match a list of selectors. Since it prevents specific items from being selected, it is known as the negation pseudo-class.

```css
  :not(h1, h2, h3, p) {
    font-size: 20px;
  }

  section > :not(p) {
    color: #fff;
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

# CSS Math Functions - `min()`, `max()`, `clamp()`

---
layout: center
---
# `min()` Function

The `min()` function contains one or more comma-separated calculations and represents the smallest value of them. We use the `min()` to set a maximum value.

```css
section {
  width: min(50%, 700px);
}
```
---
layout: center
---

# `max()` Function

The `max()` function contains one or more comma-separated calculations and represents the largest value of them. We use the `max()` to set a minimum value. 

```css
section {
  width: max(50%, 700px);
}
```

---
layout: center
---

# `clamp()` Function

The `clamp()` CSS function clamps a value between an upper and lower bound. `clamp()` enables selecting a middle value within a range of values between a defined minimum and maximum. 

It takes three parameters: _a minimum value_, _a preferred value_, and _a maximum allowed value_.

```css
clamp(minimum, value, maximum)
```

Example:

```css
p {
  font-size: clamp(300px, 50%, 800px);
}

```

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
layout: center
---

<figure class="mx-auto text-center">
<img class="mx-auto w-3/4" src="https://caniuse.bitsofco.de/static/v1/css-math-functions-1631016030324.png" alt="Data on support for the css-snappoints feature across the major browsers from caniuse.com">
<figcaption class="pt-4 underline">
  Browsers Support - Data from caniuse.com
</figcaption>
</figure>

---
layout: center
---

# Container Queries

Container Queries is one of the newest CSS feature that will allow developers to style `DOM elements` based on the size of a containing element rather than the size of the browser viewport.

```css

@container (min-width: 600px) {
  .card {
   font-size: 3em;
 }
}
 
```
---
layout: center
---

<figure class="mx-auto text-center">
<img class="mx-auto w-3/4" src="https://caniuse.bitsofco.de/static/v1/css-container-queries-1630926134618.jpg" alt="Data on support for the css-container-queries feature across the major browsers from caniuse.com">
<figcaption class="pt-4 underline">
  Browsers Support - Data from caniuse.com
</figcaption>
</figure>

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

# What does the future look like?


Expect to see more improvement and features arrive in CSS Land. 

This information is based off the snapshot from the CSS Working Group(CSS WG) Current Work.[^1]

These are features you can expect to see fully supported in the future:

 - [Container Queries](https://drafts.csswg.org/css-contain-3/) - browsers support
 - [CSS Nesting Module](https://www.w3.org/TR/css-nesting-1/)

<br>

 [^1]: [CSS Working Group](https://www.w3.org/Style/CSS/current-work)


---

# Resources

- [A Look Back at the History of CSS](https://css-tricks.com/look-back-history-css/)
- [Selectors Level 4 Draft Spec](https://drafts.csswg.org/selectors-4/)
- [Container Queries](https://css.oddbird.net/rwd/query/)
- [CSS Contain Spec](https://drafts.csswg.org/css-contain/)
- [MDN CSS Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [CSS WG Current Work](https://www.w3.org/Style/CSS/current-work)
- [Web.dev Blog](https://web.dev/blog/)
- [CSS Tricks](https://css-tricks.com/)
- [Smashing Magazine](https://www.smashingmagazine.com/)

<!--
I've only scratched the surface of Modern CSS in this talk, if you'll love to get into more depth some of the things I shared here today I will recommend you check out the following resources:
-->

---
layout: cover
class: text-center
---

# Thank You!

[Slides](https://whatsnewincss.netlify.app/) · [Demos](https://codepen.io/collection/QWjdEv) · [Links](https://linktr.ee/lauragift_)

<figure class="mx-auto text-center">
<img class="mx-auto w-1/4" src="/qr.png" alt="QR Code for Slides">
<figcaption>
</figcaption>
</figure>


<p class="text-xs">
  Slides made with 
  <a href="https://sli.dev/" target="_blank">Slidev</a>
</p>
