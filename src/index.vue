<template>
  <Navigation />
</template>

<script>
import Vue from "vue-native-core";
import { VueNativeBase } from "native-base";

Vue.use(VueNativeBase);

import Navigation from "./navigation";
export default {
  components: { Navigation },
};
</script>