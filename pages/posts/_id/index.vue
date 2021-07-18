<template>
<div>
<div class="background"></div>
  <div class="single-post-page">
    <section class="post">
      <h1>Title of the post</h1>
      <div class="post-details">
        <div>Last updated on XXX <br><br>
        Written by NAME
        </div>
      </div>
      <p>Content of the post</p>
    </section>
    <section class="post-feedback">
      <p>Please let me know what you think about this post. Send a mail to <a href="mailto:onuohac97@yahoo.com">onuohac97@yahoo.com</a></p>
    </section>
  </div>
</div>
</template>

<style scoped>
.single-post-page {
  height: 250px;
  position: relative;
  box-sizing: border-box;
  background-position: center;
  background-size: cover;
  text-align: center;
  color: #fff;
}

.background {
    background: url('https://imgur.com/AbiM1ql.jpg');
    position: fixed;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    z-index: -1;
}

.post {
  width: 100%;
}

@media (min-width: 768px) {
  .post {
    width: 37rem;
    margin: auto;
  }
}

.post-title {
  margin: 5rem;
}

.post-details {
  /* padding: 10px; */
  box-sizing: border-box;
  border-bottom: 3px solid #ccc;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}


@media (min-width: 768px) {
  .post-details {
    flex-direction: row;
  }
}

.post-details {
  color: rgb(88, 88, 88);
  margin: 0 10px;
}

.post-feedback a {
  color: red;
  text-decoration: none;
}

.post-feedback a:hover,
.post-feedback a:active {
  color: salmon;
}
</style>