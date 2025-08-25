<template>
  <heroArea v-if="!remove" />
  <button @click="changeValue">Remove from DOM</button>
  <CourseList />
  <servicesSections />
  <aboutSections />
  <whySections />
  <teamSections />
  <clientSections />
  <infoSections />
</template>

<script>
import heroArea from "@/components/heroArea.vue";
import servicesSections from "@/components/servicesSections.vue";
import aboutSections from "@/components/aboutSections.vue";
import whySections from "@/components/whySections.vue";
import TeamSections from "@/components/teamSections.vue";
import clientSections from "@/components/clientSections.vue";
import InfoSections from "@/components/infoSections.vue";
import CourseList from './components/CuorseList.vue';
export default {
  data() {
    return {
      remove: false,
    };
  },
  methods:{
    changeValue(){
      this.remove = !this.remove;
    }
  },
  components: {
    heroArea,
    servicesSections,
    aboutSections,
    whySections,
    TeamSections,
    clientSections,
    InfoSections,
    CourseList,
  },
};
</script>
