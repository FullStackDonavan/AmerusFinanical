<template>
  <PatternSection>
    <BasicSection>
      <MedicareInsuranceServicesHeroSection />
      <Breadcrumbs
        currentPageTitle="Medicare"
        parentTitle="Senior Solutions"
        parentUrl="/senior-solutions/"
      />
      <MedicareSupplementAndMedicareAdvantagePlansSection />
      <UnderstandYourMedicareOptionsSection />
      <MedicareInsuranceFrequentlyAskedQuestions
        :items="[
          {
            title: 'What is a medicare Advantage Plan:',
            content:
              'Medicare Advantage plans, also known as “MA Plans” or “Part C” are an alternative to traditional medicare. While you still have “Medicare” these plans bundle medicare part A and Part B, oftentimes even part D to give you a comprehensive plan option. These plans are regulated by the federal government and any company who wishes to offer a MA Plan must abide by strict regulations.',
          },
          {
            title: 'What does a Medicare Advantage plan Cover:',
            content:
              'MA Plans cover all of the same services that traditional medicare would cover, while often adding some additional benefits such as: Dental, Vision, Hearing, gym membership, transportation and much more.',
          },
          {
            title: 'Cost on a Medicare Advantage plan:',
            content:
              'What you pay when you see the doctor or have an inpatient/outpatient procedure depends on several factors. Medicare pays a fixed amount to the Insurer each month for your services, and the plan must abide with certain boundaries, but each medicare advantage plan can charge different out of pocket cost and even have different rules by which you can obtain services, so long as they stay with the boundaries set forth by Medicare',
          },
          {
            title: 'Are my Prescriptions covered?',
            content:
              'While not all MA Plans offer Part D (prescription drug coverage), most do. Each plan chooses the copay and or coinsurance for drugs based on a tier rating. This information can be found in your plan formulary.',
          },
          {
            title:
              'Can I have both a Medicare Supplement and a Medicare Advantage plan:',
            content:
              'Medicare Supplements do not in unison with Medicare Advantage plans. If you are enrolled in a Medicare Advantage plan and choose to enroll in a stand alone PDP plan, you will be disenrolled from your medicare advantage plan and return to original medicare',
          },
        ]"
      />

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