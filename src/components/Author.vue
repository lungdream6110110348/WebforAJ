<template>
  <div class="author content has-text-centered">
    <g-image
      alt="Author image"
      class="image"
      src="~/assets/images/author.jpg"
    />

    <h1 v-if="showTitle">
      Pumin Singhapon
    </h1>

    <p>Student at Prince of Songkhla Universiry (PSU)</p>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {
  props: {
    showTitle: {
      type: Boolean,
      default: true,
    },
  },
};
</script>
