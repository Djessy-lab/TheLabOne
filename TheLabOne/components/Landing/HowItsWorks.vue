<template>
  <div v-if="imgArg" class="mx-auto rounded-3xl" :style="{ width: imgArgWidth + '%', height: imgArgHeight + 'rem' }">
    <img :class="imageClass" :src="imgArg">
  </div>
</template>


<script>
export default {
  name: 'HowItsWorks',
  props: {
    imgArg: { type: String, default: "" },
    imgArgShadow: { type: Boolean, default: false },
    imgArgRounded: { type: Boolean, default: false },
    imgArgPosition: { type: String, default: 'center' },
    imgArgFit: { type: String, default: 'contain' },
    imgArgWidth: { type: String, default: '50' },
    imgArgHeight: { type: String, default: '50' },
  },
  computed: {
    imageClass() {
      let classes = `object-${this.imgArgFit} object-${this.imgArgPosition} w-full h-full`;
      if (this.imgArgShadow) classes += ' shadow-2xl';
      if (this.imgArgRounded) classes += ' rounded-xl';
      return classes;
    },
  }
}
</script>
