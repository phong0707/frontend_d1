<template>

        <div class="box">
          <div class="img-box">
            <img :src="image" alt="">
          </div>
          <div class="detail-box">
            <h5>
              {{ title }}
            </h5>
            <p>
                {{ des }}
            </p>
          </div>
        </div>

</template>
<script>
export default {
    props:['title', 'des', 'image']
}
</script>
