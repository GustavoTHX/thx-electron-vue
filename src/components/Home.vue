<template>
  <v-container fluid>
    <v-row justify-md="space-around" align-content="center">
      <v-col cols="12" md="6">
        <v-row justify="center">
          <v-col cols="12" md="10" sm="12">
            <v-img src="../assets/logo/Logo-THX.png"></v-img>
          </v-col>
          <v-col cols="12" md="10" sm="12">
            <p>
              Nesses 11 anos de jornada nos tornamos especialistas no segmento
              de transporte de cargas fechadas (Lotação FTL), urgentes e
              itinerantes.
            </p>
          </v-col>
          <v-col cols="12" md="10" sm="12">
            <p>
              Nos últimos 3 anos
              <strong>atendemos mais de 100 empresas</strong> nacionais e
              multinacionais com um volume de
              <strong>mais de 45 mil embarques</strong> (caminhões carregados).
            </p>
          </v-col>
        </v-row>
      </v-col>
      <v-divider vertical></v-divider>
      <v-col cols="12" md="6" sm="12">
        <v-form>
          <v-container>
            <v-row justify="center" class="login">
              <v-img src="../assets/logo/Logo-THX.png" class="imgLogo"></v-img>
              <v-col cols="12" md="12" sm="12" xs="12">
                <v-text-field
                  label="Email"
                  :rules="rules"
                  hide-details="auto"
                ></v-text-field>
              </v-col>
              <v-col cols="12" md="12" sm="12" xs="12">
                <v-text-field
                  label=" Senha"
                  :rules="rules"
                  hide-details="auto"
                ></v-text-field>
              </v-col>
              <v-col cols="12" md="6" sm="6">
                <v-divider></v-divider>
              </v-col>
              <v-col cols="12" md="6" sm="6">
                <v-divider></v-divider>
              </v-col>
              <v-col cols="12" md="6" sm="6">
                <v-btn size="large" block color="info">
                  <v-icon start> mdi-google </v-icon>
                  Google
                </v-btn>
              </v-col>
              <v-col cols="12" md="6" sm="5" xs="5">
                <v-btn block size="large" elevation="5"> Entrar </v-btn>
              </v-col>
            </v-row>
          </v-container>
        </v-form>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    rules: [
      (value) => !!value || "Obrigatório.",
      (value) => (value && value.length >= 3) || "Min 3 characters",
    ],
  }),
};
</script>

<style>
.login {
  background-color: rgba(177, 177, 177, 0.24);
  border-radius: 2em;
  padding: 3em;
}

.imgLogo {
  width: 4vw;
  height: 8vh;
  margin-left: 1%;
}
</style>