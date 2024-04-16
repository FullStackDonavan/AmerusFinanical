<template>
  <BasicSection class="container mx-auto mt-20">
    <GridTwoColumns>
      <div class="px-4 sm:px-8">
        <HeadlineTwo> Medicare Supplement </HeadlineTwo>

        <BasicList>
          <ListItems>Medical Bills</ListItems>
          <ListItems>Credit Card Debt</ListItems>
          <ListItems>Funeral Costs</ListItems>
          <ListItems>Mortgage & Bills</ListItems>
        </BasicList>
        <ParagraphDescription
          >By purchasing a Senior Life Insurance policy you can save your family
          from the financial burden of providing for these expenses. This
          provides a helping hand to your loved ones during a difficult and
          stressful time.</ParagraphDescription
        >
      </div>
      <div class="px-4 sm:px-8">
        <HeadlineTwo>Benefits of Senior Whole Life Insurance</HeadlineTwo>
        <BasicList>
          <ListItems>NO Medical Exam</ListItems>
          <ListItems
            >Rates are Locked in and Guaranteed to never increase.</ListItems
          >
          <ListItems>Coverage within 48 Hours</ListItems>
          <ListItems>Coverage up to $50,0005</ListItems>
          <ListItems>Guaranteed Issue Policies Available</ListItems>
          <ListItems>Affordable Rates</ListItems>
        </BasicList>
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