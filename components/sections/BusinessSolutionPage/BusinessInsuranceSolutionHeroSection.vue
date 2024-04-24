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
          src="/images/Business-Solutions-Hero.jpg"
          alt="Happy Kids"
          quality="80"
          sizes="sm:400px md:600px lg:800px xl:1000px xxl:1500px 2xl:3000px"
          class="full-width-height"
        />
      </div>
      <div class="p-4">
        <HeadlineOneHero>
          Business Insurance Solutions Tailored to Your Needs
        </HeadlineOneHero>
        <ParagraphDescriptionHero
          >For over two decades, Amerus Financial has been at the forefront of
          delivering need-based insurance solutions to a diverse range of
          businesses, from burgeoning startups to established enterprises. Our
          team of highly qualified professionals consistently stays abreast of
          the latest trends and regulatory changes in an insurance landscape
          that is as dynamic as it is complex.</ParagraphDescriptionHero
        >
        <ParagraphDescriptionHero
          >We recognize that offering employee benefits can be both a logistical
          and financial challenge for businesses. That’s why we’ve streamlined
          the process to make it as straightforward as possible. We begin by
          deeply understanding your company’s unique requirements and
          operational intricacies. Based on this understanding, we then develop
          a tailored plan that not only meets your specific needs but also
          remains budget-friendly.</ParagraphDescriptionHero
        >
        <ParagraphDescriptionHero
          >To ensure we provide the highest quality of coverage, we partner with
          top-rated insurance carriers across the country, all of whom
          specialize in crafting innovative, effective solutions for businesses
          like yours. This collaborative approach allows us to offer
          comprehensive yet cost-effective insurance packages that stand out in
          the market.</ParagraphDescriptionHero
        >
        <ParagraphDescriptionHero
          >The trust and confidence that hundreds of companies nationwide have
          placed in us serve as a testament to the quality, reliability, and
          excellence of the insurance solutions we provide. Reach out to Amerus
          Financial today to discover why we have become the go-to source for
          business insurance solutions that genuinely
          work.</ParagraphDescriptionHero
        >
        <ParagraphDescriptionHero
          >Contact us for a customized insurance consultation today at
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
        Heading: "Business Insurance Solutions Tailored to Your Needs",
        Description:
          "For over two decades, Amerus Financial has been at the forefront of delivering need-based insurance solutions to a diverse range of businesses, from burgeoning startups to established enterprises. Our team of highly qualified professionals consistently stays abreast of the latest trends and regulatory changes in an insurance landscape that is as dynamic as it is complex. We recognize that offering employee benefits can be both a logistical and financial challenge for businesses. That’s why we’ve streamlined the process to make it as straightforward as possible. We begin by deeply understanding your company’s unique requirements and operational intricacies. Based on this understanding, we then develop a tailored plan that not only meets your specific needs but also remains budget-friendly. To ensure we provide the highest quality of coverage, we partner with top-rated insurance carriers across the country, all of whom specialize in crafting innovative, effective solutions for businesses like yours. This collaborative approach allows us to offer comprehensive yet cost-effective insurance packages that stand out in the market. The trust and confidence that hundreds of companies nationwide have placed in us serve as a testament to the quality, reliability, and excellence of the insurance solutions we provide. Reach out to Amerus Financial today to discover why we have become the go-to source for business insurance solutions that genuinely work.",
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
