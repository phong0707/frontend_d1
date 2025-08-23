<template>
    <section class="service_section layout_padding">
    <div class="service_container">
      <div class="container ">
        <div class="heading_container heading_center">
          <h2>
            Our <span>Services</span>
          </h2>
          <p>
            There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration
          </p>
        </div>
        <div class="row">
          <ServiceCard v-for="(item, index) in services" :key="index" :name="item.name" :des="item.des" :image="item.image" />
          
        </div>
        <div class="btn-box">
          <a href="">
            View All
          </a>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import ServiceCard from '@/components/cards/ServiceCard.vue';

export default {
  components: {
    ServiceCard,
  },
  data(){
    return {
      services: [
        {
          name: 'Currency Wallet',
          des: 'fact that a reader will be distracted by the readable content of a page when looking at its layout.Thepoint of using',
          image: 'images/s1.png'
        },
        {
          name: 'Security Storage',
          des: 'fact that a reader will be distracted by the readable content of a page when looking at its layout.Thepoint of using',
          image: 'images/s2.png'
        },
        {
          name: 'Expert Support',
          des: 'fact that a reader will be distracted by the readable content of a page when looking at its layout.Thepoint of using',
          image: 'images/s3.png'
        }
      ]
    }
  }
}
</script>