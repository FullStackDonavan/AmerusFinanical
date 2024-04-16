<template>
  <BasicSection class="container mx-auto mt-20">
    <div class="px-4 sm:px-8">
      <HeadlineTwo>
        {{ IntroText.Heading }}
      </HeadlineTwo>
      <ParagraphDescription>
        There are several factors that determine the amount of Life Insurance
        that you need such as:
      </ParagraphDescription>
      <BasicList>
        <ListItems
          >Annual salary and how many years your family may need it.</ListItems
        >
        <ListItems
          >Annual salary and how many years your family may need it.</ListItems
        >
        <ListItems>Children's future college</ListItems>
        <ListItems
          >Living expenses (credit cards, auto payments, etc.)</ListItems
        >
        <ListItems>Final Expenses</ListItems>
      </BasicList>

      <ParagraphDescription>
        We have a fact finding tool when you fill out the form on this page that
        will help you determine the amount of Life Insurance Protection that you
        may need.
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
        Heading: "How much life insurance do I need?",
        description:
          "When it comes to buying life insurance, the younger you are the more affordable it will be . Premiums tend to be lower for younger people and stay the same throughout the policy period. Also their may be changes in your life that present the need for Life Insurance, like getting married or having a new baby. Anytime that your loved ones would suffer financial loss in event of your unexpected death would be a good time to have life insurance.",
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