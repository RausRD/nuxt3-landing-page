<template>
  <section class="work-info-section">
    <h2>How does it work?</h2>
    <h4>Easy, fun & essential training for moms</h4>
    <UnderlineDelimiter />
    <div class="work-actions">
      <div class="work-exercises">
        <img
          src="~/assets/svg/search-icon.svg"
          alt="search"
          class="search-icon"
        />
        <div class="work-exercises-description">
          <h4>Browse exercises</h4>
          <p>
            Browse over 100 exercises with a video or picture and a description.
          </p>
        </div>
      </div>

      <div class="work-timeline">
        <img src="~/assets/svg/curve-icon.svg" alt="curve" class="curve-icon" />
        <div class="work-timeline-description">
          <h4>Create timeline</h4>
          <p>
            Take pictures along the way during and after the pregnancy to see
            the transformation.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>
.work-info-section {
  text-align: center;
  margin-bottom: 160px;
}
.work-info-section h2 {
  margin-bottom: 24px;
}

.work-info-section > h3 {
  margin-bottom: 21px;
}

.work-info-section .underline-delimiter {
  margin: 0 auto;
  margin-bottom: 60px;
}

.work-actions {
  display: flex;
}
.work-exercises,
.work-timeline {
  display: flex;
}

.search-icon,
.curve-icon {
  margin-right: 42px;
}
.work-exercises-description,
.work-timeline-description {
  display: flex;
  flex-direction: column;
  text-align: left;
}

.work-exercises-description p {
  color: var(--text-color-secondary);
  font-size: 18px;
  line-height: 28px;
}
</style>
