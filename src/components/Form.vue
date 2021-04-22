<template>
  <v-form v-model="valid">
    <v-container>
      <v-row>
        <v-col cols="12" md="4">
          <v-text-field v-model="nombre" label="Nombre" required></v-text-field>
          <v-text-field
            v-model="ApellidoPaterno"
            label="Apellido Paterno"
            required
          ></v-text-field>
          <v-text-field
            v-model="ApellidoMaterno"
            label="Apellido Materno"
            required
          ></v-text-field>
          <v-text-field v-model="Edad" label="Edad" required></v-text-field>
          <v-text-field
            v-model="Ocupacion"
            label="Ocupacion"
            required
          ></v-text-field>
          <v-text-field
            v-model="SalarioMensual"
            label="Salario Mensual"
            required
          ></v-text-field>
          <v-text-field
            v-model="ModeloVehiculo"
            :counter="4"
            label="Modelo Vehiculo"
            required
          ></v-text-field>
          <v-container>
            <v-btn color="primary" v-on:click="handleSave">Guardar</v-btn>
            <v-btn color="primary">Nuevo</v-btn>
            <v-btn color="primary">Eliminar</v-btn>
          </v-container>
        </v-col>
      </v-row>
    </v-container>
  </v-form>
</template>
<script>
export default {
  name: "Form",
  methods: {
    handleSave() {
      console.log("handleSave");
    },
  },
  data() {
    return {};
  },
};
</script>
