<template>
  <transition v-bind="$attrs"
    appear
    mode="in-out"
    enter-active-class="animated fadeIn"
    leave-active-class="animated fadeOut">
    <div v-if="visible">
      <slot/>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'Fade',

  data: () => ({
    visible: false,
  }),

  mounted() {
    console.log('hit mounted')
    setTimeout(() => this.visible = true, 1000)

  },

  unmounted() {
    this.visible = false;

    console.log('hit unmounted')
  }
};
</script>
