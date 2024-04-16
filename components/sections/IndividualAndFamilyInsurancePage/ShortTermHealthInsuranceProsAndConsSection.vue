<template>
  <BasicSection class="container mx-auto mt-20">
    <GridTwoColumns>
      <div class="px-4 sm:px-8">
        <HeadlineTwo class="text-center">Pros:</HeadlineTwo>
        <ParagraphDescription>No Enrollment Periods</ParagraphDescription>
        <BasicList>
          <ListItems
            >With Short term plans you can shop anytime of year and even have
            coverage effective the next day.</ListItems
          >
        </BasicList>

        <ParagraphDescription>Economical Premiums</ParagraphDescription>
        <BasicList>
          <ListItems
            >Premiums are not based on household size and income such as a
            marketplace plan. Therefore these plans can be a fraction of the
            cost of the plans on the marketplace</ListItems
          >
          <ListItems>Broad Networks</ListItems>
          <ListItems
            >Oftentimes have large networks of Doctors and Hospitals for you to
            choose from.</ListItems
          >
        </BasicList>

        <ParagraphDescription>Customizable</ParagraphDescription>
        <BasicList>
          <ListItems
            >Short Term Health plans can be customized to meet your individual
            needs.</ListItems
          >
        </BasicList>
      </div>
      <div class="px-4 sm:px-8">
        <HeadlineTwo class="text-center">Cons:</HeadlineTwo>

        <ParagraphDescription
          >Pre-existing coverage limitations</ParagraphDescription
        >
        <BasicList>
          <ListItems
            >You may be denied coverage if you have any pre-existing conditions.
            If you are accepted for coverage you may have claims related to your
            condition denied</ListItems
          >
        </BasicList>

        <ParagraphDescription>Policy maximum coverage</ParagraphDescription>
        <BasicList>
          <ListItems
            >Policies may have annual limits and lifetime maximums on coverage
            benefits.</ListItems
          >
        </BasicList>

        <ParagraphDescription>Not ACA Compliant</ParagraphDescription>
        <BasicList>
          <ListItems
            >Do not cover preventative care free of charge as an exchange
            plan.</ListItems
          >
        </BasicList>

        <ParagraphDescription>ACA Subsidies don’t apply</ParagraphDescription>
        <BasicList>
          <ListItems
            >There are no government subsidies that apply to premiums and tax
            credits.</ListItems
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