<template>
  <heroArea />
  <services-sections />
  <about-sections />
  <why-sections />
  <team-sections />
  <client-sections />
  <info-sections />
</template>

<script>
import heroArea from "@/components/heroArea.vue";
import servicesSections from "@/components/servicesSections.vue";
import aboutSections from "@/components/aboutSections.vue";
import whySections from "./components/whySections.vue";
import TeamSections from "./components/teamSections.vue";
import ClientSections from "./components/clientSections.vue";
import InfoSections from "./components/infoSections.vue";
export default {
  components: {
    heroArea,
    servicesSections,
    aboutSections,
    whySections,
    TeamSections,
    ClientSections,
    InfoSections,
  },
};
</script>
