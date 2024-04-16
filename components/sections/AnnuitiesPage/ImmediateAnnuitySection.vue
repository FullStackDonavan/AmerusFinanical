<template>
  <BasicSection class="container mx-auto mt-20">
    <div class="p-4 sm:p-8">
      <HeadlineTwo>{{ IntroText.Headline }}</HeadlineTwo>
      <ParagraphDescription>
        {{ IntroText.description }}
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
        Headline: "Immediate Annuity",
        description:
          "This type of annuity is usually used by someone who is already in retirement, getting ready to retire, or just came into a windfall such as an inheritance or lottery and they want to protect their money while providing an income for themselves each month. An immediate annuity needs a large investment to be beneficial. The average age someone buys this type of annuity is usually between 65 and 70 years old. If you had a million dollars cash laying around and you put it into this type of annuity, you would immediately start collecting monthly payments that would total about $65,000 a year for 20 years (or life depending on the type you purchase). You’d earn your principal back in about 15 years.",
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