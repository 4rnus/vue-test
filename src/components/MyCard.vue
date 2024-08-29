<template lang="">
    <div class="card">
        <!-- <img src="https://static.vecteezy.com/system/resources/thumbnails/011/675/374/small_2x/man-avatar-image-for-profile-png.png" alt="Avatar" style="width:100%">
        <div class="container">
            <h4><b>User</b></h4> 
            <p>Test</p> 
        </div>

        <img src="https://tr.rbxcdn.com/bda19769d1f2e4000ccf01a4e2d6ba55/420/420/Hat/Webp" alt="Avatar" style="width:100%">
        <div class="container">
            <h4><b>Mbappe</b></h4> 
            <p>Teenage Mutant Ninja Turtles</p> 
        </div>
        <img src="../assets/SIUUU.png" alt="Avatar" style="width:100%">
        <div class="container">
            <h4><b>CR Ronaldo</b></h4> 
            <p>SIUUUU</p> 
        </div> -->
        <img :src="image" alt="name" style="width:100%">
        <div class="container">
          <h4><b>{{ name }}</b></h4>
          <p>{{ nickname }}</p>
          <p>{{ tel }}</p>
          <p>{{ email }}</p>
        </div>

    </div>
</template>

<script>
export default {
    props: ['id', 'name', 'nickname', 'tel', 'email', 'image']
}
</script>

<style scoped>
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  /* width:100%; */
}

.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

.container {
  padding: 2px 16px;
}
</style>