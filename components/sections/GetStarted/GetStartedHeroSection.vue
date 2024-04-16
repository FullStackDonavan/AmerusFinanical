<template>
  <SectionContainer class="bg-cover bg-center background text-center">
    <GridTwoColumns>
      <div>
        <ParagraphSubHeadingHero>
          {{ IntroText.SubHeading }}
        </ParagraphSubHeadingHero>
        <HeadlineOneHero>
          {{ IntroText.Heading }}
        </HeadlineOneHero>
        <ParagraphDescriptionHero>
          {{ IntroText.Description }}
        </ParagraphDescriptionHero>
      </div>
      <div>
        <RegisterForm />
      </div>
    </GridTwoColumns>
  </SectionContainer>
</template>

<script>
export default {
  name: "Homepage Hero Section",
  data() {
    return {
      IntroText: {
        SubHeading:
          "Join our community and start planning your next adventure.",
        Heading: "Get Started with Good Time Travel Today!",
        Description:
          "Ready to embark on your next journey? Sign up with Good Time Travel today and gain access to exclusive deals, personalized trip recommendations, and hassle-free booking options. Our user-friendly sign-up form makes it easy to create an account and start exploring our wide range of transportation services. Whether you're planning a group outing, corporate event, or school trip, we've got you covered. Join now and experience the convenience and reliability of Good Time Travel for all your transportation needs.",
      },
      Featured: [
        {
          id: 1,
          title: "Unmatched Comfort",
          description:
            "Travel in style and relaxation with our luxurious reclining seats and spacious interiors, ensuring a smooth and enjoyable ride for all passengers.",
        },
        {
          id: 2,
          title: "Convenient Amenities",
          description:
            "Stay connected and entertained throughout your journey with onboard flat screen monitors and charging ports, providing entertainment and power at your fingertips.",
        },
        {
          id: 3,
          title: "Expert Service",
          description:
            "Our dedicated and friendly staff are committed to providing top-notch service, from assistance with loading luggage to ensuring a safe and pleasant travel experience for all.",
        },
      ],
      CTA: {
        to: "/get-started",
        text: "Get Started Now!",
      },
    };
  },
};
</script>

<style scoped>
.background {
  background-image: url("/img/charter-bus.jpg");
}
</style>
