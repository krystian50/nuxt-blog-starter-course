<template>
  <div>
    <TestComponent />
  </div>
</template>

<script>
import test from '~/articles/test.md'

export default {
  components: {
    TestComponent: test.vue.component
  }
}
</script>
