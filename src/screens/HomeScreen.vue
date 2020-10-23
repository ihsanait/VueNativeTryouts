<template>
  <view>
    <text>{{ title }}</text>
    <button title="Go to screen1" :on-press="goToScreen"></button>
  </view>
</template>

<script>
export default {
  data() {
    return {
      title: "Home Screen Title",
    };
  },
  props: {
    navigation: {
      type: Object,
    },
  },
  methods: {
    goToScreen() {
      this.navigation.navigate("Screen1")
    },
  },
};
</script>

<style>
</style>