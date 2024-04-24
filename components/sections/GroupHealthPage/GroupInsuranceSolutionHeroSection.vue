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
        <NuxtLink
          to="https://portal.benefitalign.com/brokerengage/amerusfinancial/small-business-health-insurance/health?clearSession=True&isAnonymousQuote=True"
          target="_blank"
          rel="noopener noreferrer"
          class="inline-block py-2.5 px-8 text-sm text-white bg-indigo-600 hover:bg-indigo-800 focus:outline-none focus:ring-4 focus:ring-blue-300 font-medium rounded-lg dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
        >
          Get A Quote
        </NuxtLink>
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
