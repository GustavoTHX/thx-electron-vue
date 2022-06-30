<template>
  <v-form>
    <v-container>
      <v-row justify="center" class="sign-up">
        <v-img src="../assets/logo/Logo-THX.png" class="imgLogo"></v-img>
        <v-col cols="12" md="12" sm="12" xs="12">
          <v-text-field
            label="Email"
            :rules="rules"
            hide-details="auto"
            variant="solo"
          ></v-text-field>
        </v-col>
        <v-col cols="12" md="12" sm="12" xs="12">
          <v-text-field
            label=" Senha"
            :rules="rules"
            hide-details="auto"
            variant="solo"
          ></v-text-field>
        </v-col>
        <v-col cols="12" md="12" sm="12" xs="12">
          <v-text-field
            label="Confirma a Senha"
            :rules="rules"
            hide-details="auto"
            variant="solo"
          ></v-text-field>
        </v-col>
        <v-col cols="12" md="6" sm="6">
          <v-divider></v-divider>
        </v-col>
        <v-col cols="12" md="6" sm="6">
          <v-divider></v-divider>
        </v-col>
        <v-col cols="12" md="12" sm="12">
          <v-row justify="center">
            <v-col cols="12" md="6" sm="6">
              <v-btn
                block
                size="x-large"
                elevation="5"
                variant="outlined"
                color="info"
                >Cadastrar-se</v-btn
              >
            </v-col>
          </v-row>
        </v-col>
        <v-col cols="12" md="12" sm="12">
          <v-row justify="center">
            Não tem conta ?&ensp;
            <p class="text-decoration-underline font-weight-black">
              Registra-se
            </p>
            <signUpVue />
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </v-form>
</template>

<script>
export default {};
</script>

<style>
.sign-up {
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