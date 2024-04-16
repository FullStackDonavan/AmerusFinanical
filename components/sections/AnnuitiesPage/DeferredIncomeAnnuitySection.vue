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
        Headline: "Deferred Income Annuity",
        description:
          "This type of annuity can be had for as little as $5,000 to $10,000. Then you can add to it every month until you retire. The calculations for payments are made based on the input you promise to send and your initial investment, plus interest, subtracting fees, and other costs. Many people who have maxed out their 401K and IRA contributions, plus already have plenty of access to other cash for emergencies, like to purchase this type of annuity to ensure a set monthly payment for their retirement years to offset risks from other investments.",
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