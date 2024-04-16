<template>
  <PatternSection>
    <BasicSection>
      <InsuranceServicesHeroSection />
      <Breadcrumbs currentPageTitle="Insurance Services" />

      <BasicSection>
        <div class="mx-8">
          <!-- Card -->
          <GridThreeColumns>
            <div
              class="mx-auto mb-4 bg-indigo-300 dark:bg-indigo-900 shadow-lg rounded-lg"
              v-for="Service in Services"
              :key="Service.title"
            >
              <div class="px-6 py-5">
                <div class="flex items-start">
                  <img :src="Service.image" class="mr-4" width="250" />
                  <!-- Card content -->
                  <div class="flex-grow truncate">
                    <!-- Card header -->
                    <div
                      class="w-full sm:flex justify-between items-center mb-3"
                    >
                      <!-- Title -->
                      <h2
                        class="text-2xl leading-snug font-extrabold text-gray-50 truncate mb-1 sm:mb-0"
                      >
                        {{ Service.title }}
                      </h2>
                    </div>
                    <!-- Card body -->
                    <div
                      class="flex items-end justify-between whitespace-normal"
                    >
                      <!-- Paragraph -->
                      <div class="max-w-md text-indigo-100">
                        <p class="mb-2">
                          {{ Service.excerpt }}
                        </p>
                      </div>
                      <!-- More link -->
                      <nuxt-link
                        class="flex-shrink-0 flex items-center justify-center text-indigo-600 w-10 h-10 rounded-full bg-gradient-to-b from-indigo-50 to-indigo-100 hover:from-white hover:to-indigo-50 focus:outline-none focus-visible:from-white focus-visible:to-white transition duration-150 ml-2"
                        :to="Service.url"
                      >
                        <span class="block font-bold"
                          ><span class="sr-only">Read more</span> -></span
                        >
                      </nuxt-link>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </GridThreeColumns>
        </div>
      </BasicSection>
      <GetAnswersToYourQuestions />
    </BasicSection>
  </PatternSection>
</template>

<script>
export default {
  name: "Home Page",
  data() {
    return {
      Services: [
        {
          title: "Individual & Family",
          excerpt:
            "Tailored plans for family security. Life and health coverage ensuring peace of mind for your loved ones' future.",
          image: "/images/FamilyAndIndividual.jpg",
          url: "/individual-health-insurance/",
        },
        {
          title: "Senior Solutions",
          excerpt:
            "Confident retirement with personalized support. Medicare, long-term care coverage for worry-free golden years",
          image: "/images/Senior-Solutions.jpg",
          url: "/senior-solutions/",
        },
        {
          title: "Business Solutions",
          excerpt:
            "Safeguard business assets with tailored coverage. Liability, employee benefits ensuring growth and protection for enterprises.",
          image: "/images/Business-Solutions.jpg",
          url: "/business-solutions/",
        },
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