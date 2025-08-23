<template>
    <div class="col-md-4 ">
            <div class="box ">
              <div class="img-box">
                <img :src="image" alt="">
              </div>
              <div class="detail-box">
                <h5>
                  {{ name }}
                </h5>
                <p>
                    {{ des }}
                </p>
                <a href="">
                  Read More
                </a>
              </div>
            </div>
          </div>
</template>
<script>
export default {
    props:['name','des','image']
}
</script>