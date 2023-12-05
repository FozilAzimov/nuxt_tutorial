<template>
  <div>
    <div>Header Page</div>
    <div>{{ content }}</div>
    <button @click="refresh">Refresh</button>
  </div>
</template>

<script>
export default {
  data () {
    return { content: 'Created at: ' + new Date() }
  },
  methods: {
    refresh () {
      this.content = new Date();
    }
  }
}
</script>