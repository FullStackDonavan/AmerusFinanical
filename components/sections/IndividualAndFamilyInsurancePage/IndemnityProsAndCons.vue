<template>
  <BasicSection class="container mx-auto mt-20">
    <GridTwoColumns>
      <div class="px-4 sm:px-8">
        <HeadlineTwo class="text-center">Pros:</HeadlineTwo>
        <ParagraphDescription>Affordable Premiums</ParagraphDescription>

        <ParagraphDescription>First Dollar Coverage</ParagraphDescription>
        <BasicList>
          <ListItems
            >You get First Dollar Coverage that covers various procedures while
            not requiring you to meet a deductible.</ListItems
          >
          <ListItems>No Enrollment Period</ListItems>
          <ListItems
            >Enrollment is not limited to an enrollment period but can applied
            for anytime during the year.</ListItems
          >
        </BasicList>

        <ParagraphDescription>Customizable</ParagraphDescription>
        <BasicList>
          <ListItems
            >You can customize your plan benefits to cover the things that are
            most important to you.</ListItems
          >
        </BasicList>

        <ParagraphDescription>Direct Payments</ParagraphDescription>
        <BasicList>
          <ListItems
            >Pays directly to a member upon a qualifying incident. Payment is
            based upon a predetermined schedule of qualifying events.</ListItems
          >
        </BasicList>
      </div>
      <div class="px-4 sm:px-8">
        <HeadlineTwo class="text-center">Cons:</HeadlineTwo>

        <ParagraphDescription>Preset Fees</ParagraphDescription>
        <BasicList>
          <ListItems
            >Indemnity plans cover medical procedures at a specific dollar
            amount. If the medical practitioner charges more than the amount
            allotted you will be responsible for the difference.</ListItems
          >
        </BasicList>

        <ParagraphDescription
          >Pre-existing condition exclusions</ParagraphDescription
        >
        <BasicList>
          <ListItems
            >Indemnity plans are subject to underwriting and do not cover
            Pre-existing conditions. Some plans will cover certain pre-existing
            conditions after a waiting period.</ListItems
          >
        </BasicList>

        <ParagraphDescription>Waiting Periods</ParagraphDescription>
        <BasicList>
          <ListItems
            >Some indemnity plans have waiting periods that must be satisfied
            before specific conditions such as cancer is covered.</ListItems
          >
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