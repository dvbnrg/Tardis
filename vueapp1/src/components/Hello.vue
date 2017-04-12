<template>
  <div class="hello">
    <h1>{{ msg }}</h1>

<table id="Tardis">
  <th v-for="column in gridColumns">
    {{column}}
  </th>
  <tr v-for="data in gridData">
    <td>{{data.first_name}}</td>
    <td>{{data.last_name}}</td>
    <td>{{data.home}}</td>
  </tr>
</table>



  </div>

  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'The Vue.js App is working!',
      input_val: '',
      counter: 0,
      searchQuery: '',
      gridColumns: ['first_name', 'last_name','home'],
      gridData: [ { first_name : 'Rose',
                     last_name  : 'Tyler',
                     home       : 'Earth' },
                   { first_name : 'Zoe',
                     last_name  : 'Heriot',
                     home       : 'Space Station W3'},
                   { first_name : 'Jo',
                     last_name  : 'Grant',
                     home       : 'Earth'},
                   { first_name : 'Leela',
                     last_name  : null,
                     home       : 'Unspecified'},
                   { first_name : 'Romana',
                     last_name  : null,
                     home       : 'Gallifrey'},
                   { first_name : 'Clara',
                     last_name  : 'Oswald',
                     home       : 'Earth'},
                   { first_name : 'Adric',
                     last_name  : null,
                     home       : 'Alzarius'},
                   { first_name : 'Susan',
                     last_name  : 'Foreman',
                     home       : 'Gallifrey'} ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
