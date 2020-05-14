<template>
  <div class="footer">
    <v-footer dark padless>
      <v-card flat tile class="indigo lighten-1 white--text text-center">
        <v-row>
          <v-col cols="12" sm="3">
            <ul class="first-list">
              <li>Jobs classified</li>
              <li>Jobs in Kenya</li>
              <li>Jobs in Nigeria</li>
              <li>Jobs in Uganda</li>
              <li>Jobs in Tanzania</li>
              <li>Jobs in Ghana</li>
            </ul>
          </v-col>
          <v-col cols="12" sm="3">
            <ul class="second-list">
              <li>Classified in Kenya</li>
              <li>Classified in Senegal</li>
              <li>Classified in Tanzania</li>
              <li>Classified in Ethopia</li>
            </ul>
          </v-col>
          <v-col cols="12" sm="3">
            <ul class="third-list">
              <li>Cars in Kenya</li>
              <li>Cars in Uganda</li>
              <li>Cars in Tanzania</li>
              <li>Cars in Nigeria</li>
              <li>Cars in Ghana</li>
            </ul>
          </v-col>
          <v-col cols="12" sm="3">
            <ul class="second-list">
              <li>Poperties Classified</li>
              <li>Poperties IN Kenya</li>
              <li>Poperties I Senegal</li>
            </ul>
          </v-col>
        </v-row>
        <v-card-text>
          <v-btn
            v-for="icon in icons"
            :key="icon"
            class="mx-4 white--text"
            icon
          >
            <v-icon size="34px">{{ icon }}</v-icon>
          </v-btn>
        </v-card-text>

        <v-divider></v-divider>

        <v-card-text class="white--text">
          {{ new Date().getFullYear() }} —
          <span class="white-text"><strong>Jobbersearch</strong></span>
        </v-card-text>
      </v-card>
    </v-footer>
  </div>
</template>

<script>
export default {
  data: () => ({
    icons: ["mdi-facebook", "mdi-twitter", "mdi-linkedin", "mdi-instagram"],
  }),
};
</script>
<style>
.footer {
  margin-top: 400px;
}
.indigo {
  width: 100%;
}
.white--text {
  text-align: center;
}

.mx-4 {
  margin: 10px;
  background-color: red;
}
.mx-4:first-child {
  background-color: #4267b2;
}

.mx-4:last-child {
  background-color: green;
}
li {
  list-style-type: none;
  font-size: 15px;

  font-weight: bold;
  padding: 7px;
  margin: 10px;
}
.first-list {
}
</style>
