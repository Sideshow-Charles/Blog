<template>
  <div class="home-page">
    <div class="background"></div>
    <section class="main-header">
      <h1> All You Need To Know In The World Of Sports... </h1>
    </section>

    <PostList />

  </div>
</template>

<script>
import PostList from '../components/posts/PostList.vue'
export default {
  components: {
    PostList
  }
}
</script>

<style scoped>
/* .background {
    background: url('https://imgur.com/AbiM1ql.jpg');
    position: fixed;
    width: 100vw;
    height: 100vh;
    z-index: -1;
    top: 0;
    left: 0;
} */

.main-header {
  height: 150px;
  position: relative;
  /* padding: 5px; */
  box-sizing: border-box;
  background-position: center;
  background-size: cover;
  text-align: center;
}

.main-header h1 {
  margin: 5rem auto;
  font-size: 1.5rem;
  color: #000;
  padding: 10px;
  border-radius: 10px;
  box-sizing: border-box;
  text-align: center;
}

/* .post-preview {
    margin-bottom: 3rem;
  } */

@media (min-width: 768px) {
  .main-header h1 {
    font-size: 2rem;
  }
}
</style>
