<template>
  <BasicSection class="container mx-auto mt-20">
    <GridTwoColumns>
      <div class="px-4 sm:px-8">
        <!-- <ParagraphSubHeading>
          {{ IntroText.SubHeading }}
        </ParagraphSubHeading> -->
        <HeadlineTwo>Indemnity</HeadlineTwo>
        <ParagraphDescription>
          A fixed indemnity plan is one that pays a set amount of money for any
          medical services you receive. So, for example, if your plan specifies
          a $5000 per day benefit for a Hospital Stay then your plan will pay
          the specified amount outlined in the policy whether the bill is more
          or less. If the bill is more, then you would be responsible for the
          excess charges if it is less then the remaining monies would be yours
          to keep. Because the benefit is preset and paid out regardless of what
          the total bill for the qualified service might be, fixed indemnity
          insurance is sometimes called fixed benefit insurance or fee for
          service insurance. Flexed Indemnity plans are good for those who want
          affordable coverage that they can customize to meet their individual
          needs.
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
          src="/images/Indemnity.jpg"
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