<template>
  <table class="table">
    <thead>
      <tr>
        <th scope="col">#</th>
        <th scope="col">Nombre</th>
        <th scope="col">Apellido</th>
        <th scope="col">RUT</th>
        <th scope="col">Edad</th>
        <th scope="col">Fecha de Nacimiento</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="(persona, $index) of personas" :key="$index">
        <td>{{ $index }}</td>
        <td>{{ persona.nombre }}</td>
        <td>{{ persona.apellido }}</td>
        <td>{{ persona.rut }}</td>
        <td>{{ persona.edad }}</td>
        <td>{{ persona.fechaDeNacimiento }}</td>
      </tr>
    </tbody>
  </table>
</template>

<script>
export default {
  name: "App",
  data: () => ({
    personas: [
      {
        nombre: "Julian",
        apellido: "Espinoza",
        rut: "23.567.940-7",
        edad: 12,
        fechaDeNacimiento: "10-07-2012",
      },
      {
        nombre: "Valeska",
        apellido: "Pereira",
        rut: "18087310-4",
        edad: 29,
        fechaDeNacimiento: "11-08-2000",
      },
      {
        nombre: "Luis",
        apellido: "Gomez",
        rut: "17.094.507-8",
        edad: 70,
        fechaDeNacimiento: "01-01-1950",
      },
      {
        nombre: "Pedro",
      },
    ],
  }),
};
</script>

<style></style>