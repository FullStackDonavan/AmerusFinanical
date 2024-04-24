<template>
  <SectionContainer class="text-center">
    <GridTwoColumns>
      <div>
        <NuxtImg
          format="webp"
          src="/images/MedicareInsuranceServices.jpg"
          alt="Happy Kids"
          quality="80"
          sizes="sm:1200px md:1200px lg:2000px xl:2000px xxl:2500px 2xl:3000px"
        />
      </div>
      <div class="p-4">
        <HeadlineOneHero>
          {{ IntroText.Heading }}
        </HeadlineOneHero>
        <ParagraphDescriptionHero>
          {{ IntroText.Description }}
        </ParagraphDescriptionHero>
        <SeniorMedicareQuoteForm tag="SeniorMedicareInsuranceQuote" />
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
        Heading: "Compare Medicare Plans from up to 21 different companies",
        Description: "$0 monthly premium Medicare plans may be available.",
      },
    };
  },
};
</script>

<style scoped>
.image-container {
  width: 100%;
  height: 100%;
  overflow: hidden;
}

.full-width-height {
  width: 100%;
  height: 100%;
  object-fit: cover; /* Ensure the image covers the entire container */
}
</style>
