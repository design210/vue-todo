<template>
  <div>
      <h1>{{ this.titleText }} {{ this.count }}</h1> 
      <!-- <h1>{{ this.$store.state.todoApp.titleTxt }}</h1>   -->
  </div>
</template>

<script>
import { mapGetters, mapState } from 'vuex'

export default {
  computed: {
    ...mapGetters(['titleText']),
    ...mapState(['count']),
    //count(){return this.$store.state.todoApp.count},
  }
}


</script>

<style scoped>
h1{
  color:#2F3B52;
  font-weight:900;
  margin:2.5rem 0 1.5rem;
}

</style>
