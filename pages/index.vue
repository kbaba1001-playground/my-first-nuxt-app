<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest tech news!</h1>
    </section>
    <section class="featured-posts">
      <PostPreview
        id="1"
        thumbnail="https://www.pakutaso.com/shared/img/thumb/cafe201261762_TP_V.jpg"
        title="Hello there!"
        previewText="This my first post!"
      />
      <PostPreview
        id="2"
        thumbnail="https://www.pakutaso.com/shared/img/thumb/cafe201261762_TP_V.jpg"
        title="Hello there - second post"
        previewText="This my first post!"
      />
      <PostPreview
        id="3"
        thumbnail="https://www.pakutaso.com/shared/img/thumb/cafe201261762_TP_V.jpg"
        title="Hello there - third post"
        previewText="This my first post!"
      />
    </section>
  </div>

</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
  components: {
    PostPreview
  }
}

</script>

<style scoped>
.intro {
  height: 300px;
  background-image: url('~assets/images/cafe201261762_TP_V4.jpg');
  color: white;
}

.post-preview {
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #ccc;
  background-color: white;
  width: 90%;
}

a {
  text-decoration: none;
  color: black;
}

@media (min-width: 850px) {
  .post-preview {
    width: 400px;
    margin: 10px;
  }
}

.post-thumbnail {
  width: 100%;
  height: 200px;
  background-position: center;
  background-size: cover;
}

</style>
