<template>
  <PatternSection>
    <BasicSection>
      <LifeInsuranceServicesHeroSection />
      <Breadcrumbs
        currentPageTitle="Life Insurance"
        parentTitle="Individual Health Insurance"
        parentUrl="/individual-health-insurance/"
      />
      <WhatIsLifeInsuranceSection />
      <WhatAreTheDifferentTypesOfLifeInsuranceSection />
      <WhatTypeOfLifeInsuranceIsGoodForMeSection />
      <WhenDoINeedToPurchaseLifeInsuranceSection />
      <HowMuchLifeInsuranceDoINeedSection />

      <LifeInsuranceFrequentlyAskedQuestions
        :items="[
          {
            title: 'How Do I Get Lower Life Insurance Rates?',
            content:
              'The best way to save on life insurance is to buy it when you\'re young and healthy. You\'ll likely get a lower premium which stays the same throughout the policy period. Also it is important that you get your quotes from an agency that works with many different companies. This allows you to shop for the lowest rates for your particular age and health risk.',
          },
          {
            title: 'At what age should I buy life insurance?',
            content:
              'You should buy life insurance when your death would cause financial pain to someone that you care about.',
          },
          {
            title: 'How long should my term policy be for?',
            content:
              'Here are some factors to think about when gauging your life insurance term. 1.The length of your mortgage term. 2. When your last child will graduate college. 3. When your partner or spouse plans to retire. 4.Car payments. 5. Student loans. Your life insurance term should be for the length of time that it takes to pay off your outstanding debts..',
          },
          {
            title: 'How often should I review my life insurance coverage?',
            content:
              'Experts advise you to review your life insurance coverage at least once every two years to insure that you have adequate coverage to protect your family in event of your death. In addition every milestone in life such as a marriage, a new baby, a new mortgage etc.. should warrant a review.',
          },
        ]"
      >
      </LifeInsuranceFrequentlyAskedQuestions>
      <GetAnswersToYourQuestions />
    </BasicSection>
  </PatternSection>
</template>

<script>
export default {
  name: "Home Page",
  data() {
    return {
      listAmenities1: [
        { title: "Lorem ipsum dolor sit amet" },
        { title: "Lorem ipsum dolor sit amet" },
        { title: "Lorem ipsum dolor sit amet" },
        { title: "Lorem ipsum dolor sit amet" },
        { title: "Lorem ipsum dolor sit amet" },
      ],
      listAmenities2: [
        { title: "Lorem ipsum dolor sit amet" },
        { title: "Lorem ipsum dolor sit amet" },
        { title: "Lorem ipsum dolor sit amet" },
        { title: "Lorem ipsum dolor sit amet" },
      ],
    };
  },
};
</script>
<style>
ul li span {
  /*
     * We want the bullets outside of the list,
     * so the text is aligned. Now the actual bullet
     * is outside of the list’s container
     */
  list-style-position: outside !important;

  /*
     * Because the bullet is outside of the list’s
     * container, indent the list entirely
     */
  /* margin-left: 1em; */
}
.svg svg {
  width: 100px;
}
.logoSection {
  height: 300px;
}
</style>