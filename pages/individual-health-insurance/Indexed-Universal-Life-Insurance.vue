<template>
  <BasicSection>
    <AnnuitiesServicesHeroSection />

    <Breadcrumbs
      currentPageTitle="Pressure Washing"
      parentTitle="Services"
      parentUrl="/Services/"
    />

    <ImmediateAnnuitySection />
    <DeferredIncomeAnnuitySection />
    <FixedAnnuitySection />
    <VariableAnnuitySection />

    <ImportantFeaturesToAFixedAnnuitySection />

    <AnnuitiesInsuranceFrequentlyAskedQuestions
      :items="[
        {
          title: 'What Is An Annuity?',
          content:
            'An annuity is a financial contract between an insurance company and a buyer — typically an investor or retiree. In exchange for a lump sum or monthly payments toward the principal, an insurance company will pay out income through a series of payments or a one-time lump sum.',
        },
        {
          title: 'What Does it Mean to Be Tax-deferred?',
          content:
            'A unique benefit to an annuity is the death benefit. Should an annuity owner die before their annuity disburses all payments, the remaining assets can transfer to a spouse or surviving beneficiary. If you choose not to have a beneficiary, upon your death all remaining annuity assets will be surrendered to the issuing insurance company.',
        },
        {
          title: 'Will a Beneficiary Have to Pay Taxes on the Annuity?',
          content:
            'Yes, annuity payments disbursed to a spouse or beneficiary will be treated as taxable income.',
        },
        {
          title: 'How Soon Can I Withdraw From My Annuity Savings?',
          content:
            'Annuity owners can begin withdrawing money from their annuity by the age of 59½ without having to pay an early withdrawal fee. Some annuity contracts offer a surrender period, or an amount of time an investor has to wait before withdrawing funds from their annuity account. If money is withdrawn before that time, you will be subject to paying a surrender charge.',
        },
        {
          title: 'Why Invest in an Annuity vs. a Mutual Fund?',
          content:
            'Mutual funds follow the market conditions. While they may offer a higher rate of return if conditions are positive, they also carry higher risk of losing income and interest. Annuities, however, guarantee a steady, low-risk stream of income no matter the market conditions. They also have the ability to grow tax-deferred over time.',
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
    return {};
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