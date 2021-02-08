<template>
      <div class="tab-bar-item" @click="itemClick">
          <div v-if="!isActive" ><slot name="tabBarImg"></slot></div>
          <div v-else><slot name="tabBarImgActive"></slot></div>

          <div :class="{aciveClass:!isActive}"><slot name="tarBarContent"></slot></div>
          
  </div>    
</template>

<script>


export default {
  name: 'tarbaritem',
  data(){
 return {
    
 }
  },
  components: {
    
  },
  props:{
      path:String
  },
  methods:{
      itemClick(){
          this.$router.push(this.path);
          this.$store.commit("increament")
      }
  },
  computed:{
    isActive(){
        return this.$route.path.includes(this.path)?true:false
    }
  }
}
</script>

<style>

.tab-bar-item img{
width: 25px;
height: 25px;
}
.tab-bar-item{
  flex: 1;
    text-align: center;
   height: 49px;
}
.aciveClass{
    color: pink;
}
</style>
