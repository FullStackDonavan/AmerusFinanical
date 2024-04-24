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
          src="/images/dental-insurance-banner.jpg"
          alt="Happy Kids"
          quality="80"
          sizes="sm:400px md:600px lg:800px xl:1000px xxl:1500px 2xl:3000px"
          class="full-width-height"
        />
      </div>
      <div class="p-4">
        <HeadlineOneHero>
          Senior Solutions for Your Unique Needs
        </HeadlineOneHero>
        <SeniorDentalQuoteForm tag="SeniorDentalInsuranceQuote" />
      </div>
    </GridTwoColumns>
  </SectionContainer>
</template>

<script>
export default {
  name: "HomepageHeroSection",
  data() {
    return {};
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
