<template>
  <div>
    <h1>{{ msg }}</h1>
    <button @click.prevent.default="enviar()">Clique</button>

  </div>
</template>

<script>

export default {
  name: 'hi',
  data () {
    return {
      msg: 'Hi'
    }
  },
  methods: {
    enviar() {
      this.$eventHub.$emit('evento', {'data': 'William Silva Duarte'});

    }
  }
}
</script>
