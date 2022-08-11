<template>
  <p className="message">{{message}}
       
      </p>
</template>

<script>
export default {
    name:'Message',
    data(){
        return{}
    },
    props:{
        message:{String}
    }

}
</script>

<style>

</style>