<template>
  <div>
    <span>{{ symbol }}</span>
  </div>
</template>

<script>
export default {
  props: {
    symbol: {
      type: Symbol,
      required: true,
    }
  },
}
</script>
