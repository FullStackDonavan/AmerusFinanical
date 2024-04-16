<template>
  <BasicSection class="container mx-auto mt-20">
    <GridTwoColumns>
      <div class="px-4 sm:px-8">
        <NuxtImg
          format="webp"
          src="/images/short-tearn-health.jpg"
          sizes="sm:217px md:323px lg:376px xl:504px xxl:632px 2xl:700px"
          alt="Bus Driver"
          quality="80"
          loading="lazy"
        />
      </div>

      <div class="px-4 sm:px-8">
        <!-- <ParagraphSubHeading>
          {{ IntroText.SubHeading }}
        </ParagraphSubHeading> -->
        <HeadlineTwo>Short Term Health Insurance</HeadlineTwo>
        <ParagraphDescription>
          Short-term health plans are low-cost, low-coverage plans. Short term
          health insurance plans offer major medical benefits in the case of
          unexpected accidents and illnesses. These plans are not regulated by
          the ACA law and typically do not cover Preventative Care or ACA
          Essential Benefits such as Pregnancy. These plans are for individuals
          and families and last for a defined term of up to 364 days and
          renewable for up to 36 months depending on your state, unlike
          traditional health plans which don't have time limits. What short-term
          plans cover varies widely. Federal regulations allow short-term plans
          to create their own coverage plans without any required mandates from
          the ACA.. So, you may find substance abuse treatment coverage in one
          short-term plan, while another might cover barely anything. Short Term
          Health insurance plans are Great for those that are just wanting
          coverage in the case of an unexpected medical event.
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