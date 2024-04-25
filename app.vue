<script setup lang="ts">
import { useUser } from "~/composables/useAuth";

const nuxtApp = useNuxtApp();

nuxtApp.hook("page:finish", () => {
  window.scrollTo(0, 0);
});

useHead({
  link: [{ rel: "icon", type: "image/x-icon", href: "/img/favicon.ico" }],
});

await useUser();
useSchemaOrg([
  defineLocalBusiness({
    name: "Good Time Travel",
    logo: "/logo.png",
    telephone: "+8647601263",
    address: {
      addressCountry: "US",
      postalCode: "29624",
      address: "445 E Shockley Ferry Rd",
      addressLocality: "Anderson",
      addressRegion: "South Carolina",
      streetAddress: "445 E Shockley Ferry Rd",
    },
    openingHoursSpecification: [
      {
        dayOfWeek: ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"],
        opens: "10:00",
        closes: "17:00",
      },
    ],
  }),
]);
</script>
<template>
  <NuxtLayout>
    <div class="dark:bg-indigo-950 dark:text-slate-300">
      <NuxtPage />
    </div>
  </NuxtLayout>
</template>

<style>
.iframe-container {
  position: relative;
  width: 100%;
  padding-top: 56.25%; /* 16:9 aspect ratio (divide 9 by 16 = 0.5625) */
}

.iframe-container iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
.rotate-enter-active,
.rotate-leave-active {
  transition: all 0.4s;
}

.rotate-enter-from,
.rotate-leave-to {
  opacity: 0;
  transform: rotate3d(1, 1, 1, 15deg);
}

.page-enter-active,
.page-leave-active {
  transition: all 0.2s;
}
.page-enter-from,
.page-leave-to {
  opacity: 0;
  filter: blur(1rem);
}
</style>