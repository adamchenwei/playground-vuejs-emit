<template>
  <h1>abc

    <displayer @something:done="run" />
  </h1>

</template>

<script>
import Displayer from './Displayer';

export default {
  name: 'HelloWorld',
  components: {
    Displayer,
  },
  props: {
    msg: String
  },
  methods: {
    run(data) {
      console.log('run');
      console.log(data);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
