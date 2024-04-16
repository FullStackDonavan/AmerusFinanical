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
        Headline: "DENTAL INSURANCE FOR SENIORS",
        description:
          "As we grow older, decay, inflammation, and disease are more prone to affect our gums and teeth. You may need a dental professional, experienced in Senior Dental Health problems, like osteoporosis, diabetes, heart disease, stroke, and respiratory disease. According to the Columbia University College of Dental Medicine and the American Dental Association these conditions can also affect dental health and vice-versa, dental health can affect these conditions. That is the reason why it is extremely important that you have a Dental Insurance Plan that is tailored to the needs of seniors. Not all Dental Plans are created equal and may have exclusions and limitations that come as an unwelcome surprise when you get your bill. Talk to an expert who can ask you relevant questions and customize a plan to meet your individual needs. Give Amerus Financial a Call today at 1-888-441-7891",
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