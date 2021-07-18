<template>
    <section class="featured-posts">
      <PostPreview 
      id= "1"
      thumbnail= "https://imgur.com/ik7hYfj.jpg"
      title= "Basketball"
      previewText= "Some Basketball crap"
      />


      <PostPreview 
      id= "2"
      thumbnail= "https://imgur.com/SE1tg6H.jpg"
      title= "Baseball"
      previewText= "Some Baseball crap"
      />


      <PostPreview 
      id= "3"
      thumbnail= "https://imgur.com/62003zx.jpg"
      title= "Basketball"
      previewText= "Some more basketball crap"
      />


      <PostPreview 
      id= "4"
      thumbnail= "https://imgur.com/N67hXYg.jpg"
      title= "Football"
      previewText= "Some Football crap"
      />


      <PostPreview 
      id= "5"
      thumbnail= "https://imgur.com/10NSl0r.jpg"
      title= "Rugby"
      previewText= "Some Rugby crap"/>


      <PostPreview 
      id= "6"
      thumbnail= "https://imgur.com/dHrSDps.jpg"
      title= "Golf"
      previewText= "Some Golf crap"/>

    </section>
</template>

<script>
import PostPreview from './PostPreview'
export default {
  components: {
    PostPreview
  }
}
</script>

<style scoped>
@media (min-width: 768px) {
  .main-header h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 1.5rem;
  margin-bottom: 2rem;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
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

  .featured-posts {
  display: flex;
  padding: 5px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: space-around;
  width: 100%;
}

  .post-preview {
    width: 350px;
    margin: 10px;
  }
}

.post-thumbnail {
  width: 100%;
  height: 300px;
  background-position: cover;
  background-size: cover;
}

.post-content {
  padding: 10px;
  text-align: center;
}

a:hover .post-content,
a:active .post-content {
  background-color: #ccc;
}
</style>