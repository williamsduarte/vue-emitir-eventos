<template>
  <div>
    <h1>{{ msg }}</h1>
    <Hi />
  </div>
</template>

<script>

import Hi from '@/components/Hi'

export default {
  components: {
    Hi
  },
  name: 'hello',
  data () {
    return {
      msg: 'Hello'
    }
  }
}
</script>
