<template>
  <div class="home">
    <input type="text" v-model="code">
    <button @click="getData">住所自動入力</button>
    <p>Address: {{address}}</p>
  </div>
</template>

<script>

export default {
}
</script>



<script>
export default {
  data() {
    return {
      address: ""
    };
  },
  props:["parentCOde"],
};
</script>