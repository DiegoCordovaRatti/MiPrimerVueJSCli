<template>
  <div id="app">
    <table class="table" >
      <thead>
        <tr>
          <th scope="col">#</th>
          <th scope="col">Nombre</th>
          <th scope="col">Apellido</th>
          <th scope="col">Run</th>
          <th scope="col">Nacimiento</th>
          <th scope="col">Edad</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(user, i) in users" :key="i">
          <th scope="row">{{ i+1 }}</th>
          <td v-for="(eachUser, i) in users[i]" :key="i">
            {{ eachUser }}
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
  export default {
    name: 'App',
    data() {
      return {
        users: [{
            nombre: 'Pedro',
            apellido: 'Peterson',
            run: '11.123.123-1',
            fNacimiento: '01-01-1991',
            edad: 30
          },
          {
            nombre: 'Juan',
            apellido: 'Johnson',
            run: '12.234.234-2',
            fNacimiento: '02-02-1992',
            edad: 29
          },
          {
            nombre: 'Diego',
            apellido: 'Jacobson',
            run: '13.345.345-3',
            fNacimiento: '03-03-1993',
            edad: 28
          },
          {
            nombre: 'Francisca',
            apellido: 'Franklin',
            run: '14.456.456-4',
            fNacimiento: '04-04-1994',
            edad: 27
          },
          {
            nombre: 'María',
            apellido: 'Benites',
            run: '15.567.567-5',
            fNacimiento: '05-05-1995',
            edad: 26
          },
        ],
      };
    },

  }
</script>

<style>

</style>