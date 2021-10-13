<template>
  <div class="top">
    <button @click="contact">今日の担当者</button>
    <h1>{{ member }}</h1>
  </div>
</template>

<script>
export default {
  name: "top",
  data: function() {
    return {
      members: [
        "しみず",
        "いとぐち",
        "きむら",
        "えがみ",
        "ふじむら",
        "なかむら",
        "よしおか",
        "すぎた",
      ],
      member: "",
    };
  },

  methods: {
    contact: function() {
      let getData = Math.floor(Math.random() * this.members.length);
      // let getData = choose_at_random(this.member);
      this.member = this.members[getData];
    },
  },
};
</script>
