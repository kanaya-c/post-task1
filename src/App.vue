<template>
  <div>
    <Post v-bind.sync="zip" />
  </div>
</template>

<script>
import Post from "./components/Post";
export default {
  data: function() {
    return {
      zip: {
        code: "",
        address: ""
        }
      }
  },
  components: {
    Post
  }
};
</script>