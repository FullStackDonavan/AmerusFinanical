<template>
  <PatternSection>
    <BasicSection>
      <DentalInsuranceServicesHeroSection />
      <Breadcrumbs
        currentPageTitle="Senior Dental Insurance"
        parentTitle="Senior Solutions"
        parentUrl="/senior-solutions/"
      />
      <DentalInsuranceForSeniorsSection />
      <StandardDentalPoliciesSection />
      <EnhancedDentalPoliciesForSeniorsSection />
      <TypesOfDentalPlansSection />
      <YouCanGetHelpSection />
      <DentalInsuranceFrequentlyAskedQuestions
        :items="[
          {
            title: 'True or False: Seniors Can’t Get New Cavities?',
            content:
              'False! Actually, cavities happen more frequently in adults. Why? Because Fluoride wasn’t always in water supplies and toothpaste in the past. If your teeth didn\'t get enough exposure to fluoride when you were a child, your teeth may be subject to more cavities. Old fillings are target areas for tooth decay. As we get age, our gums tend to recede, exposing tooth roots. Tooth enamel guards the roots and without its protection your teeth are more susceptible to decay.',
          },
          {
            title: 'Why Are My Teeth Super Sensitive to Hot and Cold?',
            content:
              'This can happen to anyone, no matter their age. Your gum tissue recedes, exposing the sensitive root. Temperature extremes may negatively affect these roots. As a quick remedy, rise with a fluoride mouthwash, or switch to a toothpaste made for sensitive teeth. If your problem is severe or continues, ask your dentist for help, he may seal or bond the roots or even suggest a soft tissue graft. This procedure uses material, either man-made or from another area of your mouth, to protect exposed roots.',
          },
          {
            title: 'Can I still get braces, as a Senior?',
            content:
              'There are no age limitations for correcting misaligned (crooked) teeth. Any age can improve their dental appearance or bite. Your dentist or orthodontist can fit you for braces. It’s more common than you think.',
          },
          {
            title: 'What to do if my teeth feel loose?',
            content:
              'Many things can cause this to happen. It may be a bite or clenching issue. It could be a sign of bone loss from gum disease. Talk to your dentist if you are experiencing this. You may need to see a periodontist, a specialist in the mouth\'s gums and bones. Be ready to discuss your  medical history and your oral hygiene habits. Diabetes can also affect your gums and teeth.',
          },
          {
            title: 'Smoking and Oral Health',
            content:
              'If you’re a long time smoker, at the least you’re prone to bad breath and stained teeth. It may take longer to recover from a pulled tooth and periodontal treatment. The best solution is to quit smoking as soon as possible, please speak to your dentist about your dental health. Not only does age raise your chances of oral cancer, long-term smoking ads to the likelihood of you contracting oral cancer. If you discover a wound or sore area on your tongue, or anywhere in your mouth, watch it carefully and quickly have it examined.',
          },
          {
            title: 'Dealing with Dentists and Dementia',
            content:
              'Dementia patients are typically more alert in the morning, so this is the best time to schedule their appointment. Be specific when telling them where they are going and why. Alert the dentist ahead of time about your friend\'s condition. Communication always makes a visit go smoother. If possible, have a family member go with you to the appointment who is able to make treatment decisions if the patient is unable. Regular dentist visits may help diagnose if any procedures are needed, as speed up the process to have work done as soon as possible. This way, if the disease gets worse, your friend should only need simpler maintenance treatments',
          },
          {
            title: 'Why do I have to go to the dentist if I have no teeth?',
            content:
              'As you age, your teeth may develop unseen problems. It’s recommended for seniors to visit the dentist at least once a year for a full oral preventative exam. Your dentist will check for signs of oral cancer and other medical problems of the mouth, head, and neck. If you have dentures, they will also be checked for fit, and routinely cleaned.',
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