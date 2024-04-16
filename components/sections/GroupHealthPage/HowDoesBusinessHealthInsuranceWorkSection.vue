<template>
  <BasicSection class="container mx-auto mt-20">
    <GridTwoColumns>
      <div class="px-4 sm:px-8">
        <NuxtImg
          format="webp"
          src="/images/Group-Health-Insurance-Excerpt.jpg"
          sizes="sm:217px md:323px lg:376px xl:504px xxl:632px 2xl:700px"
          alt="Happy Kids"
          quality="80"
          loading="lazy"
        />
      </div>
      <div class="px-4 sm:px-8">
        <HeadlineTwo>{{ IntroText.Headline }}</HeadlineTwo>
        <ParagraphDescription>
          Here are few things that you should know about Business Health
          Insurance.
        </ParagraphDescription>
        <BasicList>
          <ListItems>Business Health Insurance is guaranteed issue.</ListItems>
          <ListItems
            >You have to have at least one emplyee to Qualify for
            coverage.</ListItems
          >
          <ListItems
            >You are required to contribute to your employees
            premiums.</ListItems
          >
          <ListItems
            >You do not have to want until your anniversary date to change your
            coverage.</ListItems
          >
        </BasicList>
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
        Headline: "How Does Business Health Insurance Work?",
        description:
          "Amerus Financial Group operates as an independant insurance agency with a focus on Health Insurance, Annuities, Life Insurance, and Employee Benefits. Our goal is to forge lasting connections with our clients, a commitment facilitated by our outstanding customer service. In line with this, we proudly collaborate with premier carriers in the industry, specifically selecting those whose business ideals align seamlessly with ours.",
      },
    };
  },
};
</script>