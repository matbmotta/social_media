<template>
  <div>
    <div>
      <base-button type="primary">Button</base-button>
      <base-button type="primary" icon="ni ni-bag-17">With icon</base-button>
      <base-button type="primary" icon="ni ni-atom"></base-button>
    </div>

    <div>
      <div class="row">
        <div class="col-md-12">
          <base-input placeholder="name@example.com"></base-input>
        </div>
        <div class="col-md-6 offset-md-3">
          <base-input placeholder="Disabled" disabled></base-input>
        </div>
      </div>
      <div class="row">
        <div class="col-md-6">
          <base-input placeholder="Birthday" addon-left-icon="ni ni-zoom-split-in"></base-input>
      </div>
      <div class="col-md-6">
        <base-input placeholder="Birthday" addon-right-icon="ni ni-zoom-split-in"></base-input>
      </div>
      </div>
      <div class="row">
        <div class="col-md-6">
          <base-input placeholder="Success" :valid="true"></base-input>
        </div>
        <div class="col-md-6">
          <base-input placeholder="Error input" :valid="false"></base-input>
        </div>
      </div>
    </div>
    
  </div>
</template>

<script>
// @ is an alias to /src
import BaseButton from '@/components/BaseButton.vue'
import BaseInput from '@/components/BaseInput.vue'

export default {
  name: 'About',
  components: {
    BaseButton,
    BaseInput

  }
}
</script>
