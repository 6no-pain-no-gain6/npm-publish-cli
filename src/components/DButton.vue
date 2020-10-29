<template>
  <div >
    <button @click="handleC">{{text}}</button>
  </div>
</template>

<script>
export default {
  props:{
    text:{
      type:String,
      default(){return '按钮'}
    },
    handleC:{
      type:Function,
      default(){
        return function(){
          console.log('按钮被点击了')
        }
      }
    }
  },
  name:'DButton',
  data () {
    return {
    }
  },

  methods: {

  },

  mounted () {
    window.app=this
  }

}
</script>

<style lang='scss' scoped>

</style>
