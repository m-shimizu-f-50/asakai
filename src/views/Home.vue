<template>
  <div>
    <h1>朝会アプリ</h1>
    <button @click="transition">スタート</button>
  </div>
</template>

<script>
export default {
  name: "home",
  methods:{
    transition:function(){
      this.$router.push('/Top')
    }
  }
};
</script>

<style scoped>
button {
  border: 1px solid #333;
  background-color: #333;
  color: #fff;
  padding: 10px 20px;
  margin-top: 10px;
}
</style>
