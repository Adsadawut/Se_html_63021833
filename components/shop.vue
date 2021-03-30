<template>
  <div class="flex bg-yellow-300 w-24 p-4 rounded-full">
      <img class="h-8 w-8" src="https://cdn.pixabay.com/photo/2015/12/23/01/07/shopping-cart-1105047_960_720.png" alt="">
      <h1>{{count}}</h1>
  </div>
</template>

<script>
export default {
    props:{
        count:{
            default:0
        }
    }

}
</script>

<style>

</style>