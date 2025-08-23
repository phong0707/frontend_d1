<template>
    <section class="why_section layout_padding">
    <div class="container">
      <div class="heading_container heading_center">
        <h2>
          Why Choose <span>Us</span>
        </h2>
      </div>
      <div class="why_container">
        <WhyCards v-for="(item,index) in whyCard" :key="index" :title="item.title" :des="item.des" :image="item.image"/>
      </div>
      <div class="btn-box">
        <a href="">
          Read More
        </a>
      </div>
    </div>
  </section>
</template>
<script>
import WhyCards from './cards/whyCards.vue';

export default {
  components:{
     WhyCards,
  },
  data(){
    return{
      whyCard:[
        {
          title:"Expert Management",
          des:"Incidunt odit rerum tenetur alias architecto asperiores omnis cumquedoloribus aperiam numquam! Eligendi corrupti, molestias laborumdolores quod nisi vitae voluptate ipsa? In tempore voluptate ducimusofficia id, aspernatur nihil. Tempore laborum nesciunt ut veniam, nemoofficia ullam repudiandae repellat veritatis unde reiciendis possimus animi autem natus",
          image:"images/w1.png"
        },
        {
          title:"Secure Investment",
          des:"Incidunt odit rerum tenetur alias architecto asperiores omnis cumquedoloribus aperiam numquam! Eligendi corrupti, molestias laborumdolores quod nisi vitae voluptate ipsa? In tempore voluptate ducimusofficia id, aspernatur nihil. Tempore laborum nesciunt ut veniam, nemoofficia ullam repudiandae repellat veritatis unde reiciendis possimus animi autem natus",
          image:"images/w2.png"
        },
        {
          title:"Instant Trading",
          des:"Incidunt odit rerum tenetur alias architecto asperiores omnis cumquedoloribus aperiam numquam! Eligendi corrupti, molestias laborumdolores quod nisi vitae voluptate ipsa? In tempore voluptate ducimusofficia id, aspernatur nihil. Tempore laborum nesciunt ut veniam, nemoofficia ullam repudiandae repellat veritatis unde reiciendis possimus animi autem natus",
          image:"images/w3.png"
        },
      ]
    }
  }
}
</script>