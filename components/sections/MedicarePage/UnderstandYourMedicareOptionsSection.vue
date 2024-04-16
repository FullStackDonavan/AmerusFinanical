<template>
  <BasicSection class="container mx-auto mt-20">
    <div class="px-4 sm:px-8">
      <HeadlineTwo
        >Understand your Medicare options with help from your AmerusFinancial
        team.</HeadlineTwo
      >
      <ParagraphDescription>
        Medicare Part A, B and D may be enough coverage for some, but for the
        majority of the population the coverage just isn’t enough. That is where
        a Medicare Advantage plan comes into play. These plans will help you
        cover your medical expenses while oftentimes giving added benefits to
        you. Each plan has its own little nuances, and what is right for me may
        not be right for you. That is why it is very important you speak with a
        licensed and certified insurance broker who can assist you in finding
        the right plan for you. Our licensed sales agents are here to listen to
        your needs to find the right Medicare plan for you.
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