<template>
  <div className="tweet"> 
    <ProfileImage  :image="user.image"/>

    <div className="body">
      <div className="top">
        
        <User :userData="user" />
        <Timestamp :timestamp="timestamp"/>
      </div>

      <message :message="message" />

      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>
<script>
import Actions from './Actions.vue'
import Message from './Message.vue'
import Timestamp from './Timestamp.vue'
import ProfileImage from './ProfileImage.vue'
import User from './User.vue'

export default {
  name:'Tweet',
    data (){
        return{}
    },
    methods:{},
    props:{
      timestamp:String,
      message:String,
      user:Object,
    },
    components:{
        Actions,
        Message,
        ProfileImage,
        Timestamp,
        User
    }
      // dataTweets:{
      //   name:{
      //     type:String,
      //     required:true,
      //   },
      //   image:{
      //     link:{
      //       type:String,
      //       default:'../assets/logo.png'
      //     },
      //     handle:{
      //       type:String,
      //       required:true
      //     },
      //     timeStamp:{
      //       type:String,
      //     },
      //     message:{
      //       type:String,
      //     }
      //   }
      // }
   
}


</script>

<style scoped>
a {
  color: #42b983;
}
</style>
