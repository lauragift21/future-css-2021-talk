<!--
A simple wrapper for embeded Codepens
Usage:
<Codepen id="luoMHjh-XcQ" />
-->

<script setup lang="ts">
defineProps<{
 link: string;
 width?: number;
 height?: number;
}>();
</script>

<template>
 <iframe
  :height="height"
  :width="width"
  scrolling="no"
  title="Codepen Embed"
  :src="link"
  frameborder="no"
  loading="lazy"
  allowtransparency="true"
  allowfullscreen="true"
  class="resize"
 >
  See the Pen
  <a :href="src">
  </a>
  by Gift Egwuenu (<a href="https://codepen.io/lauragift21">@lauragift21</a>) on
  <a href="https://codepen.io">CodePen</a>.
 </iframe>
</template>