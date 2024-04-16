<template>
  <BasicSection class="container mx-auto mt-20">
    <div class="px-4 sm:px-8">
      <HeadlineTwo>{{ IntroText.Headline }}</HeadlineTwo>
      <ParagraphDescription
        >Amerus Financial Group is an independent insurance brokerage firm
        specializing in Health Insurance, Annuities, Life Insurance and Employee
        Benefits products and services for successful businesses, individuals
        and their families. AFG strives to build long-term relationships with
        clients by providing high levels of customer service and by representing
        the industry’s top carriers whose business philosophies complement our
        own.</ParagraphDescription
      >

      <ParagraphDescription
        >Amerus Financial Group is an Insurance Agency that has been serving our
        4000 clients for more than 20 years. Amerus specializes in Innovative
        Health Insurance Solutions for Individuals and Business. We are based in
        Lakeland, Fl with agents in 13 states. Our agents are highly trained
        proffesionals that understand the dynamics of the ever changing. Health
        Insurance Marketplace. Give us a call today at +1-800-596-1474 you will
        be you did.</ParagraphDescription
      >
      <BasicList>
        <ListItems
          >Our agency has the knowledge and experience to provide innovative
          solutions for your company.</ListItems
        >
        <ListItems
          >Our commitment to customer service affords you peace of mind knowing
          that if any problems arise we will deal directly with your employees
          and take the burden from your shoulders.</ListItems
        >
        <ListItems
          >We offer a state of the Art Enrollment system as well as professional
          agent to guide your employees through the enrollment
          process.</ListItems
        >
        <ListItems
          >We are committed to providing you the support and guidence you need
          to navigate through the world of employee benefits.</ListItems
        >
      </BasicList>
    </div>
    <GridThreeColumns>
      <div
        class="mx-auto my-4 bg-indigo-300 dark:bg-indigo-900 shadow-lg rounded-lg"
        v-for="Service in Services"
        :key="Service.title"
      >
        <div class="px-6 py-5">
          <div class="flex items-start">
            <!-- Card content -->
            <div class="flex-grow truncate">
              <!-- Card header -->
              <div class="w-full sm:flex justify-between items-center mb-3">
                <!-- Title -->
                <h2
                  class="text-2xl leading-snug font-extrabold text-gray-50 truncate mb-1 sm:mb-0"
                >
                  {{ Service.title }}
                </h2>
              </div>
              <!-- Card body -->
              <div class="flex items-end justify-between whitespace-normal">
                <!-- Paragraph -->
                <div class="max-w-md text-indigo-100">
                  <p class="mb-2">
                    {{ Service.excerpt }}
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </GridThreeColumns>
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
      IntroText: {
        SubHeading:
          "Secure Your Future: Amerus Financial Group - Your Independent Insurance Agency for Health, Annuities, Life, and Employee Benefits",
        Headline: "Why Amerus Financial Group ?",
        description:
          "Amerus Financial Group operates as an independant insurance agency with a focus on Health Insurance, Annuities, Life Insurance, and Employee Benefits. Our goal is to forge lasting connections with our clients, a commitment facilitated by our outstanding customer service. In line with this, we proudly collaborate with premier carriers in the industry, specifically selecting those whose business ideals align seamlessly with ours.",
      },
      Services: [
        {
          title: "Fully Insured Health Insurance",
          excerpt:
            "This is simply an insurance program that all of the health claims risk is assumed by the Insurance Company and typically is utilized by groups that have health concerns or have an older workforce. Over the past several years companies have trended away from these plans opting instead to go with self funded or level funded plans.",
          image: "/images/FamilyAndIndividual.jpg",
        },
        {
          title: "Self Funded Health Insurance Plans",
          excerpt:
            "A Self Funded, or Self-Insured plan, is one in which the employer assumes the financial risk for providing health care benefits to its employees. In practical terms, Self-Insured employers pay for claims out-of-pocket as they are presented instead of paying a pre-determined premium to an insurance carrier for a Fully Insured plan. Typically, a self-insured employer will set up a special trust fund to earmark money (corporate and employee contributions) to pay incurred claims. These plans are usually sold to large organizations that benefit from having enough insured to mitigate the financial risks associated with the plan.",
          image: "/images/Senior-Solutions.jpg",
        },
        {
          title: "Level Funded Health Insurance Plans",
          excerpt:
            "A level funded health plan (also known as a partially self-funded plan) is a type of health insurance plan that combines the cost savings and customization of self-funding with the financial safety and predictability of fully funded plans. These plans have become increasingly popular in recent years for small business owners who want the benefits of a self funded program without any of the risk. Small business owners have experienced huge savings compared to traditional fully insured plans.",
          image: "/images/Business-Solutions.jpg",
        },
      ],
    };
  },
};
</script>