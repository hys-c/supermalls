<template>
  <div id='tab-bar'>
     <slot></slot>
  </div>
</template>

<script>
export default {
  components: {},
};
</script>

<style>
#tab-bar {
  display: flex;
  background-color: #f6f6f6;
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.3);
}
</style>