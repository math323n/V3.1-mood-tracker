<template>
  <emojis />

  <article class="bg-white p-5 rounded mb-5">
    <!-- <svg>
      <use :xlink:href="`#${rating}`" />
    </svg> -->
    <h1 class="font-bold">{{ title }}</h1>
    <p class="text-gray-400">{{ date }}</p>
    <p>{{ description }}</p>
    <p>Rating: {{ rating }}</p>
  </article>
</template>

<script>
import Emojis from "../misc/emojis.vue";
export default {
  name: "episodeCard",
  props: {
    title: String,
    description: String,
    date: String,
    rating: Number,
  },
  components: {
    Emojis,
  },
};
</script>