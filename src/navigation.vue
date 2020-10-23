<template>
  <view class="container">
    <AppNavigator />
  </view>
</template>

<script>
import HomeScreen from "@/screens/HomeScreen";
import Screen1 from "@/screens/Screen1";
import Screen2 from "@/screens/Screen2";
import { createAppContainer, createStackNavigator } from "vue-native-router";

const StackNavigator = createStackNavigator(
  {
    Home: HomeScreen,
    Screen1: Screen1,
    Screen2: Screen2,
  },
  {
    initialRouteName: "Home",
  }
);

const AppNavigator = createAppContainer(StackNavigator);

export default {
  components: {
    AppNavigator,
  },
};
</script>

<style>
.container {
  background-color: white;
  flex: 1;
}
</style>
