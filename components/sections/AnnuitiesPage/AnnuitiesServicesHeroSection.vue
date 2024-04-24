<template>
  <SectionContainer class="text-center">
    <GridTwoColumns>
      <div>
        <!-- <NuxtImg
          format="webp"
          src="/images/charter-bus.jpg"
          alt="Happy Kids"
          quality="80"
          sizes="sm:1200px md:1200px lg:2000px xl:2000px xxl:2500px 2xl:3000px"
        /> -->
        <NuxtImg
          format="webp"
          src="/images/annuities.jpg"
          alt="Happy Kids"
          quality="80"
          sizes="sm:400px md:600px lg:800px xl:1000px xxl:1500px 2xl:3000px"
          class="full-width-height"
        />
      </div>
      <div class="p-4">
        <ParagraphSubHeadingHero>
          {{ IntroText.SubHeading }}
        </ParagraphSubHeadingHero>
        <HeadlineOneHero>
          {{ IntroText.Heading }}
        </HeadlineOneHero>
        <ParagraphDescriptionHero>
          {{ IntroText.Description }}
        </ParagraphDescriptionHero>
        <IndividualFamilyIndexedUniversalLifeInsuranceQuoteForm
          tag="IndividualFamilyIndexedUniversalLifeInsuranceQuote"
        />
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
        SubHeading: "Experience the Differnece ",
        Heading: "A Company Truly Commited To Your Future",
        Description:
          "At Amerus Financial we are serious about putting the needs and desires of our clients before anything else. We take the time to carefully conside your individual circumstances before making any reccomendations. Our experienced planners take pride in searching out solutions to complex needs and making sure that we offer sound financial advise. With over 4,000 satisfied clients at Amerus Financial Group we strive to go above and beyond your expectations.",
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
