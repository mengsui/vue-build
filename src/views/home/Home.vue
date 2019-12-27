<template>
  <div>
      <div>
          语文：<input v-model="chineseScore"/>
      </div>
        <div>
          英语：<input v-model="englishScore"/>
      </div>
      <div>
          {{totalScore}}
      </div>
  </div>
</template>
<script>
export default {
  // js部分
  data() {
    return {
      chineseScore: 0,
      englishScore: 0,
    }
  },
  computed:{
    totalScore(){
      return this.chineseScore + this.englishScore
    }
  }
}
</script>