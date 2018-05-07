<template>
  <div id="app">
   <Hello />
   <Word />
  </div>
</template>

<script>
import Hello from '@/components/Hello'
import Word from '@/components/Word'

export default {
  components: {
    Hello,
    Word
  },
  name: 'app'
}
</script>

