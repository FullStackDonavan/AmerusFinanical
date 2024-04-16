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
          >Endodontics: Root canals, or the removal of a tooth’s decayed or
          diseased pulp, are the most common use of endodontics. This may
          require a specialist.</ListItems
        >
        <ListItems
          >Periodontics: Periodontal disease comes in many forms and could end
          up destroying supporting bones around the teeth. Treatment may include
          the placement of dental implants and treatment for inflammation. A
          specialist is often required.</ListItems
        >
        <ListItems
          >Dentures: This typically requires many extractions, making it a major
          procedure, possibly involving multiple visits. Certain family dentists
          now fit patients for dentures. Specialty offices are more familiar
          with the process and sometimes offer a smoother process.</ListItems
        >
        <ListItems
          >Implants: Some adults who have lost a small number of teeth due to an
          accident or decay might get dental implants. Implants may eliminate
          the need for a bridge since the implant looks, feels, and works like a
          regular tooth. An oral surgeon rather than your family dentist
          typically does this procedure.</ListItems
        >
        <ListItems
          >Orthodontia: This type of service uses braces to align crooked teeth.
          Most family dentists offer orthodontia.</ListItems
        >
        <ListItems
          >Cosmetic services: Bonding, whitening, and veneers are sometimes
          covered under certain dental policies. Most family dentists offer
          whitening.</ListItems
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
        Headline: "ENHANCED DENTAL POLICIES FOR SENIORS",
        description:
          "Some dental insurance plans cover a percentage of the costs for services beyond routine exams and fillings. Some examples include (but aren’t limited to):",
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