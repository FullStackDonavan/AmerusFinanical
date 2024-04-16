<template>
  <SectionContainer class="text-center">
    <GridTwoColumns>
      <div>
        <!-- <NuxtImg
          format="webp"
          src="/images/charter-bus.jpg"
          alt="Happy Kids"
          quality="80"
          sizes="sm:1200px md:1200px lg:2000px xl:2000px xxl:2500px 2xl:3000px"
        /> -->
        <NuxtImg
          format="webp"
          src="/images/amerus-financial-consultation.jpg"
          alt="Happy Kids"
          quality="80"
          sizes="sm:400px md:600px lg:800px xl:1000px xxl:1500px 2xl:3000px"
          class="full-width-height"
        />
      </div>
      <div class="p-4">
        <ParagraphSubHeadingHero>
          {{ IntroText.SubHeading }}
        </ParagraphSubHeadingHero>
        <HeadlineOneHero>
          {{ IntroText.Heading }}
        </HeadlineOneHero>
        <ParagraphDescriptionHero>
          {{ IntroText.Description }}
        </ParagraphDescriptionHero>
        <CardDeckThreeColumns class="hidden sm:block">
          <Card
            v-for="Feature in Featured"
            :key="Feature.id"
            :title="Feature.title"
            :description="Feature.description"
            :to="Feature.to"
            :text="Feature.text"
          />
        </CardDeckThreeColumns>
      </div>
    </GridTwoColumns>
  </SectionContainer>
</template>

<script>
export default {
  name: "HomepageHeroSection",
  data() {
    return {
      IntroText: {
        SubHeading:
          "Schedule a Consultation for Comprehensive Insurance Solutions and Personalized Guidance",
        Heading: "Experience Exceptional Customer Care with Amerus Financial",
        Description:
          "Amerus Financial aims to cultivate enduring partnerships with our clients through exceptional customer care and by affiliating ourselves with leading industry carriers that share our values and business ethos. Schedule a consultation with one of our approachable, reliable advisors, and you’ll receive comprehensive answers to all your queries. Together, we’ll design an insurance plan that aligns perfectly with your needs.",
      },
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
};
</script>

<style scoped>
.image-container {
  width: 100%;
  height: 100%;
  overflow: hidden;
}

.full-width-height {
  width: 100%;
  height: 100%;
  object-fit: cover; /* Ensure the image covers the entire container */
}
</style>
