<template>
  <BasicSection class="container mx-auto mt-20">
    <GridTwoColumns>
      <div class="px-4 sm:px-8">
        <!-- <NuxtImg
          format="webp"
          src="/images/happy-kids.jpg"
          sizes="sm:217px md:323px lg:376px xl:504px xxl:632px 2xl:700px"
          alt="Happy Kids"
          quality="80"
          loading="lazy"
        /> -->
        <video controls>
          <source
            src="/videos/Amerus-Financial-Group-Insurance-Agency.mp4"
            type="video/mp4"
          />
          Your browser does not support the video tag.
        </video>
      </div>
      <div class="px-4 sm:px-8">
        <HeadlineTwo>{{ IntroText.Headline }}</HeadlineTwo>
        <ParagraphDescription>
          {{ IntroText.description }}
        </ParagraphDescription>
      </div>
    </GridTwoColumns>
  </BasicSection>
</template>

<script>
export default {
  name: "Ideal Customers Section",
  props: {
    title: String,
    description: String,
    mediaFirst: Boolean,
    subTitle: String,
  },
  data() {
    return {
      IntroText: {
        SubHeading:
          "Secure Your Future: Amerus Financial Group - Your Independent Insurance Agency for Health, Annuities, Life, and Employee Benefits",
        Headline: "What We Provide",
        description:
          "Amerus Financial Group operates as an independant insurance agency with a focus on Health Insurance, Annuities, Life Insurance, and Employee Benefits. Our goal is to forge lasting connections with our clients, a commitment facilitated by our outstanding customer service. In line with this, we proudly collaborate with premier carriers in the industry, specifically selecting those whose business ideals align seamlessly with ours.",
      },
    };
  },
};
</script>