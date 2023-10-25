<template>
  <section class="blog-posts-section">
    <h2>Our blog posts</h2>
    <UnderlineDelimiter />
    <div class="blog-posts">
      <img
        src="~/assets/img/running-post.png"
        alt="running post"
        class="blog-main-post"
      />
      <div class="blog-secondary-posts">
        <img src="~/assets/img/walking-post.png" alt="running post" />
        <img src="~/assets/img/workout-post.png" alt="workout post" />
        <img src="~/assets/img/fitness-post.png" alt="fitness post" />
        <img src="~/assets/img/therapist-post.png" alt="therapist post" />
      </div>
    </div>
    <div class="view-more">
      <span>Like what you see? View more</span>
      <button class="view-more-button">
        <img src="~/assets/svg/button-right.svg" alt="view more" />
      </button>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
.blog-posts-section {
  text-align: center;
  margin-bottom: 81px;
}

.blog-posts-section h2 {
  margin-bottom: 21px;
}
.blog-posts-section > .underline-delimiter {
  margin: 0 auto;
  margin-bottom: 60px;
}
.blog-posts {
  display: flex;
}
.blog-main-post {
  height: 604px;
  width: 604px;
}

.blog-secondary-posts {
  margin-left: 32px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.blog-secondary-posts img {
  height: 286px;
  width: 286px;
  margin-bottom: 32px;
}
.view-more {
  display: flex;
  justify-content: center;
}
.view-more > span {
  font-size: 24px;
  line-height: 160%;
}
.view-more-button {
  border: none;
  padding: 0;
  background: transparent;
  margin-left: 9px;
}
</style>
