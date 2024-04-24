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
          src="/images/FamilyAndIndividual.jpg"
          alt="Happy Kids"
          quality="80"
          sizes="sm:400px md:600px lg:800px xl:1000px xxl:1500px 2xl:3000px"
          class="full-width-height"
        />
      </div>
      <div class="p-4">
        <HeadlineOneHero>
          Individual & Family Solutions for Health Insurance
        </HeadlineOneHero>
        <ParagraphDescriptionHero>
          Navigating the increasingly complex and costly world of health
          insurance has never been more challenging, particularly given the
          industry’s uncertain future. In such times, having a trusted advisor
          to guide you through the maze of options for affordable and sufficient
          health coverage for your family is invaluable.
        </ParagraphDescriptionHero>
        <ParagraphDescriptionHero
          >AFG is recognized and certified by the Centers for Medicare &
          Medicaid Services (CMS), enabling us to assist you in qualifying for
          tax subsidies that could cover a significant portion, if not all, of
          your health insurance premiums. As the landscape of the Affordable
          Care Act (ACA) undergoes rapid changes, the importance of having an
          informed and reliable advisor by your side cannot be overstated. Our
          role is to provide you with timely guidance and answer any queries you
          may have regarding your health coverage
          options.</ParagraphDescriptionHero
        >
        <ParagraphDescriptionHero
          >We are proud to represent a roster of top-rated health insurance
          providers, including but not limited to United Healthcare, Ambetter,
          Molina, Aetna, Florida Blue, Blue Cross Blue Shield of South Carolina,
          Oscar, and Cigna. This range of partnerships ensures that we can offer
          a variety of high-quality options tailored to meet your specific
          needs.</ParagraphDescriptionHero
        >
        <ParagraphDescriptionHero
          >Don’t hesitate to secure your family’s future with affordable health
          insurance. Call us today for a no-obligation quote at
          1-888-441-7891</ParagraphDescriptionHero
        >
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
        Heading: "Individual & Family Solutions for Health Insurance",
        Description:
          "Navigating the increasingly complex and costly world of health insurance has never been more challenging, particularly given the industry’s uncertain future. In such times, having a trusted advisor to guide you through the maze of options for affordable and sufficient health coverage for your family is invaluable. AFG is recognized and certified by the Centers for Medicare & Medicaid Services (CMS), enabling us to assist you in qualifying for tax subsidies that could cover a significant portion, if not all, of your health insurance premiums. As the landscape of the Affordable Care Act (ACA) undergoes rapid changes, the importance of having an informed and reliable advisor by your side cannot be overstated. Our role is to provide you with timely guidance and answer any queries you may have regarding your health coverage options. We are proud to represent a roster of top-rated health insurance providers, including but not limited to United Healthcare, Ambetter, Molina, Aetna, Florida Blue, Blue Cross Blue Shield of South Carolina, Oscar, and Cigna. This range of partnerships ensures that we can offer a variety of high-quality options tailored to meet your specific needs. Don’t hesitate to secure your family’s future with affordable health insurance. Call us today for a no-obligation quote at 1-888-441-7891",
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
