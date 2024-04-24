<template>
  <BasicSection>
    <HeroSection
      title="Pressure Washing Services"
      description="RESTORE, RENEW, REVEAL: PRESSURE WASHING POWER"
      url="https://nuxtjs.org"
      image="/img/pressure-washing-banner.jpg"
    />

    <SeniorLifeInsuranceSolutionHeroSection tag="SeniorLifeInsuranceQuote" />
    <Breadcrumbs
      currentPageTitle="Senior Life"
      parentTitle="Senior Solutions"
      parentUrl="/senior-solutions/"
    />
    <WhatIsSeniorLifeInsuranceSection />

    <SeniorInsuranceFrequentlyAskedQuestions
      :items="[
        {
          title: 'What Is Health Insurance? ',
          content:
            'Health insurance is a type of coverage that can protect you from the full expense of regular health care, as well as the costs of medical and surgical procedures. In exchange for paying a premium, your insurance company will cover the costs of your healthcare and certain types of medical procedures.',
        },
        {
          title: 'What Does Health Insurance Cover?',
          content:
            'You may qualify for a tax credit if your income is less than 400% of FPL. If your income is between 100% and 200% of FPL you may qualify for a subsidy to help cover your deductible and out of pocket expenses.',
        },
        {
          title: 'Am I eligible for a subsidy?',
          content:
            'Health insurance can cover a variety of things, from your regular checkups and family care to your major medical expenses. The types of services that are covered will vary with different healthcare providers and plan types.',
        },
        {
          title: 'Will a Short Term Insurance plan cover my Pregnancy?',
          content:
            'There are Short term plan options that will cover a pregnancy. That being said, most short term plans will have an exclusion for pregnancy.',
        },
        {
          title: 'How do I Apply for Medicaid?',
          content:
            'You can apply in one of two ways : 1. You can go through the health insurance marketplace and let th em send your application to your state medicaid office. 2. You can also apply directly through your state agency.',
        },
        {
          title: 'What is the Affordable care act:',
          content:
            'The comprehensive health care reform law enacted in March 2010 (sometimes known as ACA, PPACA, or “Obamacare”). Make affordable health insurance available to more people. The law provides consumers with subsidies (“premium tax credits”) that lower costs for households with incomes between 100% and 400% of the federal poverty level. Expand the Medicaid program to cover all adults with income below 138% of the federal poverty level. (Not all states have expanded their Medicaid programs.) Support innovative medical care delivery methods designed to lower the costs of health care generally. Additional Information Can be obtained from Healthcare.gov',
        },
        {
          title: 'Is health insurance required by law?',
          content:
            'Individuals are no longer subject to tax penalties if they choose not to carry Health Insurance but businesses with 50 or more full time employees are still required to provide coverage to their employees.',
        },
      ]"
    />
    <GetAnswersToYourQuestions />
  </BasicSection>
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