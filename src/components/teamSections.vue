<template>
    <section class="team_section layout_padding">
    <div class="container-fluid">
      <div class="heading_container heading_center">
        <h2 class="">
          Our <span> Team</span>
        </h2>
      </div>

      <div class="team_container">
        <div class="row">
          <TeamCards v-for="(item,index) in teamCard" :key="index" :name="item.name" :role="item.role" :image="item.image"/>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import TeamCards from './cards/teamCard.vue';

export default {
  components:{
    TeamCards
  },
  data(){
    return{
      teamCard:[
        {
          name:"Joseph Brown",
          role:"Marketing Head",
          image:"images/team-1.jpg"
        },
        {
          name:"Nancy White",
          role:"Marketing Head",
          image:"images/team-2.jpg"
        },
        {
          name:"Earl Martinez",
          role:"Marketing Head",
          image:"images/team-3.jpg"
        },
         {
          name:"Josephine Allard",
          role:"Marketing Head",
          image:"images/team-4.jpg"
        },
      ]
    }
  }
}
</script>