<template>
  <BasicSection class="container mx-auto mt-20">
    <div class="p-4 sm:p-8">
      <HeadlineTwo>{{ IntroText.Headline }}</HeadlineTwo>
      <ParagraphDescription>
        You can purchase an individual dental insurance plan, for premiums
        typically ranging from $20-$60 a month. Standard policies commonly cover
        these routine procedures at a family dentist office.
      </ParagraphDescription>
      <BasicList>
        <ListItems
          >Basic cleanings and exams: Most policies entitle you to a free basic
          cleaning and comprehensive exam twice a year.</ListItems
        >
        <ListItems
          >X-rays: Dentists periodically take bitewing X-rays of your teeth.
          X-rays may be fully covered, or you might make a copayment depending
          on your dental insurance plan,. Additional X-rays of your mouth may
          require a copayment, coinsurance, or deductible.</ListItems
        >
        <ListItems
          >Fillings and extractions: Fillings and extractions usually require a
          copayment, coinsurance or deductible in most dental insurance
          plans.</ListItems
        >
        <ListItems
          >Certain Procedures : Standard individual dental insurance plans
          occasionally include partial coverage on some restorative procedures,
          such as root canals, crowns, bridges, and deep cleanings. Your plan
          may require a copayment, coinsurance or deductible for procedures and
          there may be services that are not covered at all. So you know what to
          expect at your appointment, please carefully review your insurance
          plan or speak to your insurance agent before your dental appointment.
          You might need to search for a policy that covers more extensive
          services.</ListItems
        >
      </BasicList>
    </div>
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
      colorMode: useColorMode(),
      IntroText: {
        Headline: "STANDARD DENTAL POLICIES",
        description:
          "As we grow older, decay, inflammation, and disease are more prone to affect our gums and teeth. You may need a dental professional, experienced in Senior Dental Health problems, like osteoporosis, diabetes, heart disease, stroke, and respiratory disease. According to the Columbia University College of Dental Medicine and the American Dental Association these conditions can also affect dental health and vice-versa, dental health can affect these conditions. That is the reason why it is extremely important that you have a Dental Insurance Plan that is tailored to the needs of seniors. Not all Dental Plans are created equal and may have exclusions and limitations that come as an unwelcome surprise when you get your bill. Talk to an expert who can ask you relevant questions and customize a plan to meet your individual needs. Give Amerus Financial a Call today at 1-888-441-7891",
      },
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