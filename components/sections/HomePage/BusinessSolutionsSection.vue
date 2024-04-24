<template>
  <BasicSection class="container mx-auto mt-20">
    <GridTwoColumns>
      <div class="px-4 sm:px-8">
        <!-- <ParagraphSubHeading>
          {{ IntroText.SubHeading }}
        </ParagraphSubHeading> -->
        <HeadlineTwo>
          {{ IntroText.Heading }}
        </HeadlineTwo>
        <ParagraphDescription>
          {{ IntroText.description }}
        </ParagraphDescription>
        <div
          class="flex flex-col mb-8 lg:mb-16 space-y-4 sm:flex-row sm:justify-left sm:space-y-0 sm:space-x-4"
        >
          <NuxtLink
            to="/business-solutions/"
            class="text-slate-100 hover:text-slate-300 dark:hover:text-slate-100 dark:text-slate-800 focus:outline-none focus:ring-4 focus:ring-blue-300 dark:focus:ring-amber-800 bg-blue-400 hover:bg-blue-800 dark:bg-amber-500 dark:hover:bg-amber-600 font-medium text-sm rounded-lg px-5 py-2.5 mr-2 mb-2"
          >
            Learn More
          </NuxtLink>
        </div>
      </div>
      <div class="px-4 sm:px-8">
        <NuxtImg
          format="webp"
          src="/images/Business-Solutions.jpg"
          sizes="sm:217px md:323px lg:376px xl:504px xxl:632px 2xl:700px"
          alt="Bus Driver"
          quality="80"
          loading="lazy"
        />
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
      IntroText: {
        SubHeading:
          "Empower your business to new heights with our marketing blueprint. Let us make it effortless for your customers to find you!",
        Heading:
          "Safeguarding Your Business's Success: Comprehensive Insurance Solutions for Enterprises",
        description:
          "Protect your business and its assets with our comprehensive Business Solutions. At Amerus Financial, we recognize the unique challenges businesses face in today's dynamic environment. From liability coverage to employee benefits packages, our tailored solutions are designed to mitigate risks and promote growth. Our experienced advisors work closely with you to understand your business needs and objectives, offering strategic guidance and support to help you achieve your goals. Partner with Amerus Financial to safeguard your business's success and ensure a prosperous future.",
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