<template>
  <section class="posts-list">
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
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview";

export default {
  components: {
    PostPreview
  }
};
</script>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-items: center;
}

.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
