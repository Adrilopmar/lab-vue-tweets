<template>
  <img
      :src='image'
      className="profile"
      alt="profile"
    />
</template>

<script>
export default {
    name:'ProfileImage',
    data(){
        return{}
    },
    props:{
        image:{String}
    }

}
</script>

<style>

</style>