<template>
  <v-form v-model="valid">
    <v-container>
      <v-row>
        <v-col cols="12" md="4">
          <v-text-field
            v-model="nombre"
            :rules="nameRules"
            :counter="10"
            label="Nombre"
            required
          ></v-text-field>

          <v-text-field
            v-model="ApellidoPaterno"
            :rules="nameRules"
            :counter="10"
            label="Apellido Paterno"
            required
          ></v-text-field>
          <v-text-field
            v-model="ApellidoMaterno"
            :rules="nameRules"
            label="Apellido Materno"
            required
          ></v-text-field>
          <v-text-field
            v-model="Edad"
            :rules="nameRules"
            label="Edad"
            required
          ></v-text-field>
          <v-text-field
            v-model="Ocupacion"
            :rules="nameRules"
            label="Ocupacion"
            required
          ></v-text-field>
          <v-text-field
            v-model="SalarioMensual"
            :rules="nameRules"
            label="Salario Mensual"
            required
          ></v-text-field>
          <v-text-field
            v-model="ModeloVehiculo"
            :rules="nameRules"
            label="Modelo Vehiculo"
            required
          ></v-text-field>
          <v-container>
            <v-btn color="primary">Crear</v-btn>
            <v-btn color="primary">Crear</v-btn>
            <v-btn color="primary">Crear</v-btn>
          </v-container>
        </v-col>
      </v-row>
    </v-container>
  </v-form>
</template>
<script>
export default {
  name: "Form",
};
</script>
