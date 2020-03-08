<template>
  <nuxt-link :to="'/posts/' + id" class="post-preview">
    <article>
      <div
        class="post-thumbnail"
        :style="{backgroundImage: 'url(' + thumbnail + ')'}"
      ></div>
      <div class="post-content">
        <h1>{{ title }}</h1>
        <p>{{ previewText }}</p>
      </div>
    </article>
  </nuxt-link>
</template>

<script>
export default {
  name: 'PostPreview',
  props: {
    id: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    previewText: {
      type: String,
      required: true
    },
    thumbnail: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
.post-preview {
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #ccc;
  background-color: white;
  width: 90%;
}

.post-thumbnail{
  width: 30rem;
  height: 30rem;
}
</style>
