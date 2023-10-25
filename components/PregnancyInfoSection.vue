<template>
  <section class="pregnancy-info-section">
    <img src="~/assets/svg/healthy.svg" alt="" />
    <h2>Before, during and after pregnancy</h2>
    <h4>
      The app is divided into three different stages to help you choose
      appropriate exercises. Each exercise is carefully selected to ensure safe
      and appropriate adjustments to follow the pregnancy's progress.
    </h4>
    <UnderlineDelimiter />
    <div class="before-pregnancy-block">
      <div class="before-pregnancy-description">
        <h3>Before pregnancy</h3>
        <UnderlineDelimiter />
        <p>
          Start preparing for pregnancy with safe exercises that build up a
          strong body.
        </p>
        <h4>Trimesters</h4>
        <p>
          The pregnancy is divided into first trimester, second trimester part 1
          and 2, and third trimester part 1 and 2 to provide exercises that are
          safe for each stage of the pregnancy. Each exercise comes with a video
          and a description so you can safely perform each exercise. Simple put
          in your due date and you will be taken to the proper stage.
        </p>
      </div>
    </div>
    <div class="during-pregnancy-block">
      <img src="~/assets/img/during-pregnancy.png" />
      <div class="during-pregnancy-description">
        <h3>During pregnancy</h3>
        <UnderlineDelimiter />
        <p>
          Working out during pregnancy has many benefits for both the mom and
          the baby. It can reduce back pain, help prevent gestational diabetes,
          promote good posture, strength and endurance, and also improve the
          ability to cope with labor.
        </p>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
.pregnancy-info-section {
  text-align: center;
  margin-bottom: 160px;
  position: relative;
}
.pregnancy-info-section > img {
  position: absolute;
  top: 950px;
  right: 0;
  z-index: -1;
}
.pregnancy-info-section h2 {
  margin-bottom: 24px;
}
.pregnancy-info-section > h4 {
  margin-bottom: 21px;
}

.pregnancy-info-section > .underline-delimiter {
  margin: 0 auto;
  margin-bottom: 60px;
}
.before-pregnancy-block {
  height: 683px;
  background-image: url(~/assets/img/before-pregnancy.png);
  background-size: contain;
  background-repeat: no-repeat;
  background-position: right;
  margin-bottom: 68px;
}
.before-pregnancy-description {
  text-align: left;
  padding-top: 198px;
  max-width: 556px;
}
.before-pregnancy-description p {
  color: var(--text-color-secondary);
  font-size: 18px;
  line-height: 28px;
  margin-bottom: 16px;
}
.before-pregnancy-description > h3 {
  margin-bottom: 13px;
}
.before-pregnancy-description > h4 {
  margin-bottom: 5px;
}
.before-pregnancy-description .underline-delimiter {
  margin: 0;
  margin-bottom: 24px;
}
.before-pregnancy-banner img {
  height: 683px;
}
.during-pregnancy-block {
  height: 652;
  display: flex;
}
.during-pregnancy-block > img {
  height: 652px;
}

.during-pregnancy-description {
  text-align: left;
  padding-top: 262px;
  padding-left: 90px;
  /* max-width: 556px; */
}
.during-pregnancy-description h3 {
  margin-bottom: 13px;
}
.during-pregnancy-description .underline-delimiter {
  margin: 0 auto 24px 0;
}
</style>
