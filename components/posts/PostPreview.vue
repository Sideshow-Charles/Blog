<template>

    <nuxt-link :to="'/posts/' + id" class="post-preview">
      <article>
        <div class="post-thumbnail" 
        :style="{backgroundImage: 'url(' + thumbnail +')'}"></div>
        <div class="post-content">
        <h1>{{title}}</h1>
        <h4>{{previewText}}</h4>
        </div>
      </article>
      </nuxt-link>
</template>

<script>
export default {
    // name: PostPreview,
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
    margin-bottom: 3rem;
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