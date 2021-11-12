<template>
  <ul id="links" class="menu bg-base-100" :class="[isMobile ? '' : 'horizontal']">
    <slot></slot>
    <li>
      <a href="#"> Collections </a>
    </li>
    <li>
      <a href="#"> Menu</a>
    </li>
    <li>
      <a href="#"> Women </a>
    </li>
    <li>
      <a href="#"> About </a>
    </li>
    <li>
      <a href="#"> Contact </a>
    </li>
  </ul>
</template>

<script>
export default {
  props: ["isMobile"],
  data() {
    return {};
  },
};
</script>
<style scoped>
#links li a:focus {
  border-color: hsl(26, 100%, 55%);
  border-bottom-width: 3px;
  background-color: white;
}
</style>
