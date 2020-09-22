<template>
  <div>
     <base-button type="primary">Button</base-button>
      <base-button type="primary" icon="ni ni-bag-17">With icon</base-button>
      <base-button type="primary" icon="ni ni-atom"></base-button>
  </div>
</template>

<script>
// @ is an alias to /src
import BaseButton from '@/components/BaseButton.vue'

export default {
  name: 'About',
  components: {
    BaseButton
  }
}
</script>
