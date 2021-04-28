<template>
  <!-- App.vue -->

  <v-app>
    <v-parallax
      height="1000"
      src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"
    >
      <!--
    <v-navigation-drawer app>
      
    </v-navigation-drawer>
            -->
      <!--
    <v-app-bar app>
      <v-banner>Unit Test Challenge</v-banner>
    </v-app-bar>
    -->

      <!-- Sizes your content based upon application components -->
      <v-main>
        <v-row>
          <v-col>
            <v-container>
              <v-form v-model="valid">
                <v-container>
                  <v-row>
                    <v-col cols="12" md="4">
                      <v-text-field
                        v-model="clientes.Nombre"
                        label="Nombre"
                        required
                      ></v-text-field>
                      <v-text-field
                        v-model="clientes.ApellidoPaterno"
                        label="Apellido Paterno"
                        required
                      ></v-text-field>
                      <v-text-field
                        v-model="clientes.ApellidoMaterno"
                        label="Apellido Materno"
                        required
                      ></v-text-field>
                      <v-text-field
                        v-model="Edad"
                        label="Edad"
                        required
                      ></v-text-field>
                      <v-text-field
                        v-model="clientes.Ocupacion"
                        label="Ocupacion"
                        required
                      ></v-text-field>
                      <v-text-field
                        v-model="clientes.SalarioMensual"
                        label="Salario Mensual"
                        required
                      ></v-text-field>
                      <v-text-field
                        v-model="clientes.ModeloVehiculo"
                        :counter="4"
                        label="Modelo Vehiculo"
                        required
                      ></v-text-field>
                      <v-container>
                        <v-btn color="primary" v-on:click="handleSave"
                          >Guardar</v-btn
                        >
                        <v-btn color="primary">Nuevo</v-btn>
                        <v-btn color="primary">Eliminar</v-btn>
                      </v-container>
                    </v-col>
                  </v-row>
                </v-container>
              </v-form>
            </v-container>
          </v-col>
          <v-col>
            <v-container>
              <v-data-table
                :headers="headers"
                :items="clientes"
                :items-per-page="5"
                class="elevation-1"
              ></v-data-table>
            </v-container>
          </v-col>
        </v-row>
      </v-main>

      <v-footer app>
        <!-- -->
      </v-footer>
    </v-parallax>
  </v-app>
</template>

<script>
export default {
  name: "App",
  methods: {
    handleSave() {
      var index = 0;
      console.log(this.clientes[index].Nombre);
      index = index + 1;
      this.clientes[index] = this.clientes.Nombre;
      console.log(this.clientes[index].Nombre);
    },
  },
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
