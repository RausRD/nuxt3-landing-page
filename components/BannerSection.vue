<template>
  <section class="banner-section">
    <div class="banner-info">
      <h1>Strong for life with us</h1>
      <UnderlineDelimiter />
      <p class="banner-app-info">
        The best Pre/postnatal fitness app! 100 exercises divided in before,
        during and after pregnancy. Stay strong and healthy through all stages
        of pregnancy.
      </p>
      <div class="app-download-actions">
        <div class="apple-download-button">
          <AppleDownloadButton />
        </div>
        <div class="android-download-button">
          <AndroidDownloadButton />
        </div>
      </div>
    </div>
    <div class="banner-image">
      <img src="~/assets/img/iphone-12-pro.png" alt="iphone image" />
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
.banner-section {
  height: 817px;
  background-image: url(~/assets/img/banner-background.png);
  background-size: contain;
  background-repeat: no-repeat;
  display: flex;
  padding: 106px 106px 0 106px;
  margin-bottom: 160px;
}
.banner-section .underline-delimiter {
  margin-bottom: 36px;
}

.banner-info {
  flex: 1 1 0;
}
.banner-info h1 {
  margin-bottom: 21px;
  max-height: 129px;
}

.banner-app-info {
  color: var(--text-color-secondary);
  font-size: 24px;
  line-height: 160%;
  max-height: 150px;
  margin-bottom: 36px;
}
.app-download-actions {
  display: flex;
}
.apple-download-button {
  margin-right: 40px;
}

.banner-image {
  flex: 1 1 0;
  position: relative;
}
.banner-image img {
  height: 860px;
  position: absolute;
  top: -80px;
  /* border: 1px solid black; */
}
</style>
