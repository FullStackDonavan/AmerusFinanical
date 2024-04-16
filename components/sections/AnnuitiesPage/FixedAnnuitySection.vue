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
        Headline: "Fixed Annuity",
        description:
          "The returns increase in value based on a set interest rate that is known at the time of the purchase. Usually, this is the type of annuity you get when you set up a deferred income annuity. They have better interest rates than CDs (certificates of deposit), and all the interest you earn is tax-deferred until you start receiving payments. Normally, you don’t have to choose your exact payment dates until closer to your retirement. At that time, they will work out the payments that you’ll receive after you stop paying into the fund. However, you will have an idea of what you’ll get based on interest rates, the payments you pay in monthly, plus when you start taking payments.",
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