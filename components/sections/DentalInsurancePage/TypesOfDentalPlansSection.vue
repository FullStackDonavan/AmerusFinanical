<template>
  <BasicSection class="container mx-auto mt-20">
    <div class="p-4 sm:p-8">
      <HeadlineTwo>{{ IntroText.Headline }}</HeadlineTwo>
      <ParagraphDescription>
        You can purchase an individual dental insurance plan, for premiums
        typically ranging from $20-$60 a month. Standard policies commonly cover
        these routine procedures at a family dentist office.
      </ParagraphDescription>
      <BasicList>
        <ListItems
          >Managed-care plans (PPOs: preferred provider organizations) negotiate
          fees with specific providers. These in-network providers request only
          your percentage of the cost and file any necessary claims on your
          behalf. Out of network providers that perform procedures may or may
          not be covered and if they are, it may be at a lesser
          amount.</ListItems
        >
        <ListItems
          >Indemnity plans often include a larger group of providers and you may
          be able to see the dentist of your choice. The negative side is that
          patients are often required to pay 100 percent of the bill up front
          and then submit a claim for reimbursement for the covered
          procedure.</ListItems
        >
      </BasicList>
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
        Headline: "TYPES OF DENTAL PLANS",
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