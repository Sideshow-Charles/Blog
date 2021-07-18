<template>
  <div class="admin-page">
    <section class="new-post">
      <button @click="$router.push('/admin/new-post')">New Post</button>
    </section>
    <section class="existing-posts">
      <h1>Existing Posts</h1>
      <PostList isAdmin />
    </section>
  </div>
</template>

<script>
import PostList from "../../components/posts/PostList.vue";

export default {
  components: {
    PostList,
  },
};
</script>

<style scoped>
.admin-page {
  padding: 20px;
}

.new-post {
  text-align: right;
  margin: 1rem 0;
  /* border-bottom: 2px solid #ccc; */
  padding-bottom: 10px;
}

button {
  border: none;
  background-color: green;
  color: white;
  padding: 0.7rem 0;
  width: 30%;
  font-size: 0.9rem;
  cursor: pointer;
  border-radius: 10px;
}

button:hover {
  color: white;
  background-color: rgb(10, 80, 10);
}

.existing-posts h1 {
  text-align: center;
}

@media (min-width: 768px) {
  button {
    width: 12%;
    font-size: 1rem;
  }
}
</style>