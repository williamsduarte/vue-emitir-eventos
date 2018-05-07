<template>
  <div>
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>

export default {

  name: 'word',
  data () {
    return {
      msg: 'Word'
    }
  },
  created() {
    this.$eventHub.$on('evento', function(obj) {
      console.log(obj.data)
    });
  }
}
</script>
