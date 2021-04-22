<template>
  <v-data-table
    :headers="headers"
    :items="clientes"
    :items-per-page="5"
    class="elevation-1"
  ></v-data-table>
</template>
<script>
export default {
  data() {
    return {
      headers: [
        {
          text: "Nombre",
          align: "start",
          sortable: false,
          value: "Nombre",
        },
        { text: "Apellido Paterno", value: "ApellidoPaterno" },
        { text: "Apellido Materno", value: "ApellidoMaterno" },
        { text: "Edad", value: "Edad" },
        { text: "Ocupacion", value: "Ocupacion" },
        { text: "Salario Mensual", value: "SalarioMensual" },
        { text: "Modelo Vehiculo", value: "ModeloVehiculo" },
        { text: "Seguro disponible", value: "SeguroDisponible" },
      ],
      clientes: [
        {
          Nombre: "Saul Ivan",
          ApellidoPaterno: "Soto",
          ApellidoMaterno: "Pino",
          Edad: 24,
          Ocupacion: "Estudiante / Trabajo",
          SalarioMensual: "12000",
          ModeloVehiculo: 2012,
          SeguroDisponible: "NA",
        },
      ],
    };
  },
};
</script>
