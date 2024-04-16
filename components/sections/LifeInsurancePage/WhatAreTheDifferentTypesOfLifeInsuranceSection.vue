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
        Heading: "What are the Different types of life insurance",
        description:
          "There are two main types of life insurance: term life insurance and whole life insurance. Temporary coverage is called “Term Life Insurance” this type of coverage is typically a lot less expensive and is designed to provide coverage protection for a specified period of time. Their are many terms to choose from, there is yearly term called “annual renewable term” that provides coverage for a set premium amount for one year after that it renews on an annual basis with premiums increasing accordingly. Then there is term insurance that locks in your premiums for a number of years such as 10, 15, 20 or 30 years. These policies provides level premiums throughout the term of the policy. The there is “permanent insurance” these policies are designed for premiums to remain level throughout your lifetime or until the policies are “paid up.” These policies build cash value and offer many different cash accumulation strategies and future income options that are attractive to many who purchase them. The premiums are higher than term insurance because they are level for the life of the contract. The policies are called “Whole Life Insurance” or “Universal Life Insurance.”",
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