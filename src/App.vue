<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <Home />
  <CustomCheckbox />
  <ConditionalRendering />
  <LoopsComponent />
  <ParentComponent />
  <ChildComponent />
  <ParentReuse />
  <ChildReuse />
  <HtmlBinding />
  <ClassBinding />
  <PropsDataPass />
  <ChildParentData />
</template>

<script>


// import HelloWorld from './components/HelloWorld.vue'
// import Home from './components/Home.vue'
// import CustomCheckbox from './components/CustomCheckbox.vue'
// import ConditionalRendering from './components/ConditionalRendering.vue';
// import LoopsComponent from './components/LoopsComponent.vue';
// import ParentComponent from './components/ParentComponent.vue';
// import ChildComponent from './components/ChildComponent.vue';
// import ParentReuse from './components/ParentReuse.vue';
// import ChildReuse from './components/ChildReuse.vue';
// import HtmlBinding from './components/HtmlBinding.vue';
// import ClassBinding from './ClassBinding.vue';
// import PropsDataPass from './components/PropsDataPass.vue';
import ChildParentData from './components/ChildParentData.vue';



export default {
  name: 'App',
  components: {
    // HelloWorld,
    // Home
    // CustomCheckbox
    // ConditionalRendering
    // LoopsComponent.
    // ParentComponent,
    // ChildComponent
    // ParentReuse
    // ChildReuse
    // HtmlBinding
    // ClassBinding
    // PropsDataPass
    ChildParentData
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
