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
        Heading: "When do I need to purchase Life Insurance",
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