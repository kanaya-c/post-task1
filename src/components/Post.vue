<template>
  <div>
    <input type="text" v-model="code">
    <button @click="getData">住所自動入力</button>
    <p>Address:{{address}}</p>
  </div>
</template>

<script>
import axios from "axios";
export default {
  props: {
    'Zip':{

    }
  },
  methods:
  function() {
    axios.get('https://apis.postcode-jp.com/api/v4/postcodes/1500001')
    .then(response => console.log(response));
  },
  getData() {
    this.address = this.zip;
  }
}
</script>