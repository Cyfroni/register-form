<template>
  <div class="form-group">
    <label :for="inputId" class="wedio-white">{{ name }}</label>
    <input
      class="form-control"
      :type="type"
      :id="inputId"
      :placeholder="placeholder"
      v-model="value"
      @submit="handleSubmit"
      @change="handleChange"
    />
    <p v-if="error">
      <span class="error">{{ error }}</span>
    </p>
  </div>
</template>

<script>
export default {
  props: {
    inputId: {
      type: String,
      required: true
    },
    name: {
      type: String,
      required: true
    },
    type: {
      type: String,
      required: true
    },
    placeholder: {
      type: String
    }
  },
  data() {
    return {
      error: null,
      value: ''
    }
  },
  methods: {
    validate() {
      if (this.value.length) {
        return true
      }
      this.error = 'value is required'
      return false
    },
    handleChange() {
      if (this.validate()) {
        this.error = null
      }
    },
    handleSubmit() {
      console.log(this.value)
    }
  }
}
</script>

<style>
.error {
  color: red;
}
</style>
