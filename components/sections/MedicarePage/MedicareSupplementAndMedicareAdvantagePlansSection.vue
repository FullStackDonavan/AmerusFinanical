<template>
  <BasicSection class="container mx-auto mt-20">
    <GridTwoColumns>
      <div class="px-4 sm:px-8">
        <HeadlineTwo> Medicare Supplement </HeadlineTwo>
        <ParagraphDescription>
          Original Medicare does not cover all of your medical expenses. A
          Medicare Supplement plan helps fill the expenses not covered by
          original Medicare. A Medicare supoplement may be purchased along with
          Part D presciption drug coverage.
        </ParagraphDescription>
      </div>
      <div class="px-4 sm:px-8">
        <HeadlineTwo> Medicare Advantage</HeadlineTwo>
        <ParagraphDescription>
          Medicare Advantage plans are an alternative to original medicare. A
          Medicare Advantage Plans is offered by private insurance companies.
          They often provide additional benefits that original medicare does not
          provide. These plans also may offer a paid prescription as well.
        </ParagraphDescription>
      </div>
    </GridTwoColumns>
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