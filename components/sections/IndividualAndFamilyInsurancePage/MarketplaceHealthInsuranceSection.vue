<template>
  <BasicSection class="container mx-auto mt-20">
    <GridTwoColumns>
      <div class="px-4 sm:px-8">
        <!-- <ParagraphSubHeading>
          {{ IntroText.SubHeading }}
        </ParagraphSubHeading> -->
        <HeadlineTwo> Marketplace Health Insurance ('Obama Care') </HeadlineTwo>
        <ParagraphDescription>
          The Affordable Care Act (ACA), otherwise known as Obamacare, is
          designed to make guaranteed issue health insurance plans available to
          everyone. These plans cover preexisting conditions along with a list
          of essential health benefits that don't change from plan to plan,
          known as preventative care. The ACA has established a yearly Open
          Enrollment period (Nov. 1st-Dec 15th) for enrolling in a qualified
          health plan. In most cases, if you want ACA coverage, you must enroll
          in an ACA-compliant medical plan within that period. However, if you
          experience a qualifying event or major life change outside of that
          Open Enrollment window, you may be able to enroll during a Special
          Enrollment period. Contact an agent to see if you qualify. .
        </ParagraphDescription>
        <!-- <div
          class="flex flex-col mb-8 lg:mb-16 space-y-4 sm:flex-row sm:justify-left sm:space-y-0 sm:space-x-4"
        >
          <NuxtLink
            to="/service-area-business-marketing-program"
            class="text-slate-100 hover:text-slate-300 dark:hover:text-slate-100 dark:text-slate-800 focus:outline-none focus:ring-4 focus:ring-blue-300 dark:focus:ring-amber-800 bg-blue-400 hover:bg-blue-800 dark:bg-amber-500 dark:hover:bg-amber-600 font-medium text-sm rounded-lg px-5 py-2.5 mr-2 mb-2"
          >
            Learn More About Our Program
          </NuxtLink>
        </div> -->
      </div>
      <div class="px-4 sm:px-8">
        <NuxtImg
          format="webp"
          src="/images/marketplace.jpg"
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