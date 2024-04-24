<template>
  <BasicSection class="container mx-auto mt-20">
    <CardDeckThreeColumns class="hidden sm:block">
      <QuoteCard>
        <div
          class="block overflow-hidden rounded-t-lg rounded-b-lg h-full shadow-lg bg-gray-50 text-gray-800 dark:bg-gray-800 dark:text-gray-100"
        >
          <div class="p-4 bg-blue-400 dark:bg-amber-400">
            <h2
              class="mt-2 mb-2 font-bold text-2xl font-Heading text-center text-white"
            >
              A.C.A Quote
            </h2>
          </div>
          <IndividualFamilyHealthcareInsuranceQuoteForm
            tag="HealthInsuranceACAQuote"
          />
          <div class="text-md p-3 mb-4">
            <BasicList>
              <ListItems>40 yr Male, 40 yr female, 2 children</ListItems>
              <ListItems>Deductible: $0</ListItems>
              <ListItems>PCP Copay: $8</ListItems>
              <ListItems>Specialist Copay: $15</ListItems>
              <ListItems>RX copay: $8</ListItems>
            </BasicList>
            <ParagraphDescription
              >Plan Premium with tax credit = $145.77</ParagraphDescription
            >
          </div>
          <div>
            <!-- <img :src="image" /> -->
          </div>
        </div>

        <div
          class="block overflow-hidden rounded-t-lg rounded-b-lg h-full shadow-lg bg-gray-50 text-gray-800 dark:bg-gray-800 dark:text-gray-100"
        >
          <div class="p-4 bg-blue-400 dark:bg-amber-400">
            <h2
              class="mt-2 mb-2 font-bold text-2xl font-Heading text-center text-white"
            >
              Short Term Medical
            </h2>
          </div>
          <IndividualFamilyHealthcareInsuranceQuoteForm
            tag="HealthInsuranceShortTermMedical"
          />
          <div class="text-md p-3 mb-4">
            <BasicList>
              <ListItems>40 yr Male, 40 yr female, 2 children</ListItems>
              <ListItems>Deductible: $2000</ListItems>
              <ListItems>Doctor Co-pays $30/$60</ListItems>
              <ListItems>RX: $10 Co-pay</ListItems>
              <ListItems>Up to 36 months of Coverage</ListItems>
              <ListItems>Teledoc Included</ListItems>
            </BasicList>
            <ParagraphDescription
              >Short Term Silver Plan $369.80</ParagraphDescription
            >
          </div>
          <div>
            <!-- <img :src="image" /> -->
          </div>
        </div>

        <div
          class="block overflow-hidden rounded-t-lg rounded-b-lg h-full shadow-lg bg-gray-50 text-gray-800 dark:bg-gray-800 dark:text-gray-100"
        >
          <div class="p-4 bg-blue-400 dark:bg-amber-400">
            <h2
              class="mt-2 mb-2 font-bold text-2xl font-Heading text-center text-white"
            >
              Indemnity
            </h2>
          </div>
          <IndividualFamilyHealthcareInsuranceQuoteForm
            tag="HealthInsuranceIndemnity"
          />
          <div class="text-md p-3 mb-4">
            <BasicList>
              <ListItems>40 yr Male, 40 yr female, 2 children</ListItems>
              <ListItems>Hospitalization = $3000 per day</ListItems>
              <ListItems>Surgery 100% *restrictions apply</ListItems>
              <ListItems>Emergency Room = $125 per/day</ListItems>
              <ListItems>Doctors Office Visit = $ 100 per visit</ListItems>
              <ListItems>Teledoc Included</ListItems>
            </BasicList>
            <ParagraphDescription>Plan Premium $268.00</ParagraphDescription>
          </div>
          <div>
            <!-- <img :src="image" /> -->
          </div>
        </div>
      </QuoteCard>
    </CardDeckThreeColumns>
  </BasicSection>
</template>


<script>
export default {
  name: "Ideal Customers Section",
  props: {
    title: String,
    description: String,
    mediaFirst: Boolean,
    subTitle: String,
  },
  data() {
    return {
      Featured: [
        {
          id: 1,
          title: "Individual & Family",
          description:
            "Ensure your family's future with our personalized insurance plans. From life to health coverage, we tailor solutions to meet your needs, providing security and peace of mind.",
          to: "/get-started",
          text: "Get Started Now!",
        },
        {
          id: 2,
          title: "Senior",
          description:
            "Navigate retirement confidently with our senior insurance plans. From Medicare to long-term care coverage, we offer personalized support for your golden years.",
          to: "/get-started",
          text: "Get Started Now!",
        },
        {
          id: 3,
          title: "Business",
          description:
            "Protect your business with our tailored insurance solutions. From liability coverage to employee benefits, we safeguard your interests and promote growth.",
          to: "/get-started",
          text: "Get Started Now!",
        },
      ],
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