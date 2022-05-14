<template>
  <div id="app">
    <PanelViewVue></PanelViewVue>
    <ControllerViewVue></ControllerViewVue>
  </div>
</template>

<script>
import PanelViewVue from './views/PanelView.vue';
import ControllerViewVue from './views/ControllerView.vue';
import PanelView from './views/PanelView.vue';
import ControllerView from './views/ControllerView.vue';

export default {
  name: 'App',

  components: {
    ControllerViewVue,
    PanelViewVue,
    PanelView,
    ControllerView
}
};
</script>

<style>
#app {
  text-align: center;
  margin-top: 60px;
}
</style>