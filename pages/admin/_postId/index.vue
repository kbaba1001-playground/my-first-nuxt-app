<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from "@/components/Admin/AdminPostForm";

export default {
  components: {
    AdminPostForm
  },
  data() {
    return {
      loadedPost: {
        author: "Maximilian",
        title: "My awesome Post",
        content: "Super amazing, thanks for that!",
        thumbnailLink:
          "https://www.pakutaso.com/shared/img/thumb/cafe201261762_TP_V.jpg"
      }
    };
  }
};
</script>
