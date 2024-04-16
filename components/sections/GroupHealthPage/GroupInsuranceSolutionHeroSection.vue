<template>
  <SectionContainer class="text-center">
    <GridTwoColumns>
      <div>
        <div class="video-container">
          <iframe
            class="full-width-height"
            src="https://www.youtube.com/embed/pJLJhErFHqs"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
      </div>
      <div class="p-4">
        <HeadlineOneHero>
          {{ IntroText.Heading }}
        </HeadlineOneHero>
        <ParagraphDescriptionHero>
          {{ IntroText.Description }}
        </ParagraphDescriptionHero>
      </div>
    </GridTwoColumns>
  </SectionContainer>
</template>

<script>
export default {
  name: "HomepageHeroSection",
  data() {
    return {
      IntroText: {
        Heading: "Business Health Insurance-No Obligation Quote!",
        Description:
          "For 20 years, Amerus Financial delivers tailored insurance solutions, staying updated on trends. Streamlined process, tailored plans, top-rated carriers, trusted nationwide.",
      },
    };
  },
};
</script>

<style scoped>
.video-container {
  position: relative;
  width: 100%;
  padding-top: 56.25%; /* 16:9 aspect ratio */
}

.full-width-height {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>
