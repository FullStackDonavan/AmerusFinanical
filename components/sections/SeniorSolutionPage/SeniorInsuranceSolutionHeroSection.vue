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
          src="/images/Senior-Solutions.jpg"
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
        <ParagraphDescriptionHero
          >The senior market is often inundated with a deluge of advertising and
          promotional materials, making it challenging to sift through the
          information overload to make well-informed choices. Amidst this
          cacophony, it’s easy to feel overwhelmed and unsure of which route to
          take for your financial and insurance needs.</ParagraphDescriptionHero
        >
        <ParagraphDescriptionHero
          >Here at Amerus Financial, we adopt a client-centered approach that
          starts with truly listening to you. We take the time to understand
          your unique needs, lifestyle, and financial situation. Armed with this
          understanding, we then tailor a customized solution that aligns
          specifically with your requirements and goals. Rest assured, we
          operate on a foundation of integrity; our advisors will never pressure
          you into selecting a product that doesn’t serve your best
          interests.</ParagraphDescriptionHero
        >
        <ParagraphDescriptionHero
          >Choosing to work with us means choosing a partner committed to
          treating you with the respect and dignity you rightfully deserve. We
          aim to build a long-lasting relationship founded on trust, honesty,
          and superior customer service.</ParagraphDescriptionHero
        >
        <ParagraphDescriptionHero
          >Take the first step in securing a financial and insurance plan that
          genuinely suits your needs. Contact us today for a personalized quote
          at 1-888-441-7891</ParagraphDescriptionHero
        >
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
