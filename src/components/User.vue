<template>
  <span className="user">
          <span className="name">{{userData.name}}</span>
          <span className="handle">{{userData.handle}}</span>
        </span>
</template>

<script>
export default {
    name:'User',
    data(){
        return{}
    },
    props:{
        userData:Object
    }
}
</script>

<style>

</style>