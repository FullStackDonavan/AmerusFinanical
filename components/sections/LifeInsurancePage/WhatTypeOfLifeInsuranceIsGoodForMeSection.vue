<template>
  <BasicSection class="container mx-auto mt-20">
    <div class="px-4 sm:px-8">
      <HeadlineTwo>
        {{ IntroText.Heading }}
      </HeadlineTwo>
      <ParagraphDescription>
        {{ IntroText.description }}
      </ParagraphDescription>
    </div>
  </BasicSection>
</template>

<script>
export default {
  name: "TwoColumnSection",
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
        Heading: "What type of life insurance is good for me",
        description:
          "That depends on your specific situation if you are looking for short term coverage that may provide protection for something like a mortgage or an income replacement policy while your children are at home, then typically you would look at getting a term life insurance policy. If you are looking for coverage to cover final expenses or to leave your spouse well provided for you may want to look at a permanent life insurance solution. There are many factors that go into making that decision and it is best that you go over your concerns with a licensed insurance professional who will be able to point you in the right direction.",
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