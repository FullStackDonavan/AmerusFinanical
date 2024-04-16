<template>
  <BasicSection class="container mx-auto mt-20">
    <div class="p-4 sm:p-8">
      <HeadlineTwo>{{ IntroText.Headline }}</HeadlineTwo>
      <ParagraphDescription>
        You can purchase an individual dental insurance plan, for premiums
        typically ranging from $20-$60 a month. Standard policies commonly cover
        these routine procedures at a family dentist office.
      </ParagraphDescription>
      <ParagraphDescription>
        It’s important to have dental insurance in place before an urgent need
        arises. Many seniors take daily medications that cause dry mouth, which
        can cause cavities. Insufficient nutrition can also affect your dental
        health.
        <ParagraphDescription>
          Remember that health problems, like insulin resistance or pneumonia,
          may be caused or worsened by poor dental hygiene. Intellihealth News
          Service research has even found a connection between gum disease and
          heart disease.
        </ParagraphDescription>
        <ParagraphDescription
          >Enter your zip code above if you’d like to explore your options for
          individual dental insurance plans in your area.
        </ParagraphDescription>
        <ParagraphDescription
          >This article is for informational purposes only. Nothing in it should
          be used as a substitute for professional medical advice. Always
          consult with your medical provider regarding diagnosis or treatment
          for a health condition, including decisions about the correct
          medication for your condition, as well as prior to undertaking any
          specific exercise or dietary routine. In addition, this information
          includes just some factors to consider when selecting insurance and
          may not reflect the provisions of any particular insurance product.
          Always carefully check the provisions of any insurance product you
          have or may consider purchasing.</ParagraphDescription
        >
      </ParagraphDescription>
    </div>
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
      colorMode: useColorMode(),
      IntroText: {
        Headline:
          "YOU CAN GET HELP CHOOSING AN INDIVIDUAL DENTAL INSURANCE PLAN",
        description:
          "The two most common types of individual dental insurance plans available to seniors are",
      },
    };
  },
  computed: {
    // const isDark = this.$colorMode.value === "dark";
    isDark() {
      if (this.colorMode.preference === "dark") {
        return true;
      } else {
        return false;
      }
    },
  },
};
</script>

<style scoped>
</style>