<template>
  <BasicSection class="container mx-auto mt-20">
    <GridTwoColumns>
      <div class="px-4 sm:px-8">
        <HeadlineTwo class="text-center">Pros:</HeadlineTwo>
        <ParagraphDescription>Dependant Coverage</ParagraphDescription>
        <BasicList>
          <ListItems
            >Dependants can stay on your policies until age 26.</ListItems
          >
        </BasicList>

        <ParagraphDescription>Subsidies & Tax Credits</ParagraphDescription>
        <BasicList>
          <ListItems
            >For those that qualify, Subsidies and tax credits not only bring
            down the monthly premium (Cost) of your health insurance but also
            bring down things such as Deductibles and copayments on silver
            plans. Based on your FPL (Federal Poverty Level.)</ListItems
          >
          <ListItems>No pre-existing condition limitations.</ListItems>
          <ListItems
            >Insurance companies cannot cancel your health plan due to an error
            on your application nor can they deny you coverage due to a
            pre-existing health condition that you may have.</ListItems
          >
        </BasicList>

        <ParagraphDescription>No waiting periods</ParagraphDescription>
        <BasicList>
          <ListItems
            >There is no more waiting period to be met before you or your
            dependent can see a physician. Once your policy is effective you can
            begin using the benefits immediately.</ListItems
          >
        </BasicList>

        <ParagraphDescription>Free Preventative Care</ParagraphDescription>
        <BasicList>
          <ListItems
            >All qualified marketplace plans must provide preventative care,
            free of charge to you. That means no deductibles, copayments, or
            coinsurance.</ListItems
          >
        </BasicList>

        <ParagraphDescription>No Caps</ParagraphDescription>
        <BasicList>
          <ListItems
            >All qualified health plans must cover according to the policy
            contract without a maximum benefit.</ListItems
          >
        </BasicList>
      </div>
      <div class="px-4 sm:px-8">
        <HeadlineTwo class="text-center">Cons:</HeadlineTwo>

        <ParagraphDescription>Limited Companies</ParagraphDescription>
        <BasicList>
          <ListItems
            >Due to the fact that Marketplace health plans have lost the
            majority of their risk stops, such as pre-existing condition
            waivers, many insurance companies simply cannot afford to offer
            plans on the health exchange. Therefore you are limited to certain
            companies and networks. Some counties only have one
            option.</ListItems
          >
        </BasicList>

        <ParagraphDescription
          >High Deductibles and High premiums</ParagraphDescription
        >
        <BasicList>
          <ListItems
            >For those that do not qualify for the subsidies and tax credits
            marketplace plans may be unaffordable. Customers may end up paying
            high premiums while also being stuck with a high deductible
            plan.</ListItems
          >
        </BasicList>

        <ParagraphDescription>Tax Penalties</ParagraphDescription>
        <BasicList>
          <ListItems
            >Prior to 2019, you could face large tax penalties for being
            uninsured. While this has been done away with on a federal level
            many states have begun to enforce similar mandates of their
            own.</ListItems
          >
        </BasicList>

        <ParagraphDescription>Annual Open Enrollment</ParagraphDescription>
        <BasicList>
          <ListItems
            >Once the enrollment period is closed it becomes next to impossible
            to purchase a plan on the exchange. Those looking for coverage
            outside of OEP (Open Enrollment Period - November 1, 2020 – December
            15, 2020.) must have a qualifying life event to open up an SEP
            (special Enrollment Period).</ListItems
          >
        </BasicList>

        <ParagraphDescription>Loss of Employment Coverage</ParagraphDescription>
        <BasicList>
          <ListItems
            >Due to the ACA there has been a major increase in premiums making
            group insurance coverage unaffordable for many small
            businesses.</ListItems
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