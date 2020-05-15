<template>
  <div class="form">
    <div class="container fluid">
      <h3 class="first-heading">FIND A JOB</h3>
      <v-row justify="center">
        <v-col sm="8" md="12">
          <v-container fluid>
            <v-row align="center" class="form-row">
              <v-col class="d-flex" cols="12" sm="8" id="form-content">
                <v-select
                  :items="items"
                  label="All Job Function"
                  solo
                ></v-select>
              </v-col>
              <v-col class="d-flex" cols="12" sm="8" id="form-content-1">
                <v-select :items="items" label="All industries" solo></v-select>
              </v-col>
              <v-col class="d-flex" cols="12" sm="6" id="form-content-2">
                <v-select :items="items" label="Location" solo> </v-select>
              </v-col>
              <v-col class="d-flex" cols="12" sm="2" id="form-content-3">
                <v-btn
                  class="ma-4"
                  color="orange darken-4"
                  id="form-btn"
                  dark
                  large
                >
                  <v-icon>fas fa-search </v-icon>SEARCH
                </v-btn>
              </v-col>
            </v-row>
          </v-container>
        </v-col>
      </v-row>
    </div>
    <div class="container fluid" id="subsection">
      <v-container fluid>
        <v-row justify="center">
          <v-col sm="12" md="6">
            <v-container fluid>
              <v-row justify="center">
                <v-col class="d-flex" cols="12" sm="12" id="form-content-4">
                  <v-btn
                    class="ma-6"
                    color="orange darken-4"
                    id="form-btn-2"
                    dark
                    large
                  >
                    SEARCH FILTER</v-btn
                  >
                </v-col>

                <v-card max-width="594" class="mx-auto" height="200">
                  <v-list-item color="blue darken-3" id="headline-item"
                    ><h3 class="para-heading">Government jobs in Abuja</h3>
                  </v-list-item>

                  <v-card-text>
                    <p id="first-para">2 Jobs Found</p>
                  </v-card-text>

                  <v-card-actions>
                    <v-btn
                      class="ma-6"
                      color="orange darken-4"
                      id="form-btn-2"
                      dark
                      large
                      >CREATE JOB ALERT</v-btn
                    >

                    <v-spacer></v-spacer>
                  </v-card-actions>
                </v-card>
              </v-row>
            </v-container>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    items: ["Foo", "Bar", "Fizz", "Buzz"],
  }),
};
</script>
<style>
.form {
  background-color: #1565c0;
  height: 300px;
}

.first-heading {
  color: white;
  text-align: center;

  font-size: 20px;
}
.container {
}
.form-row {
  margin-top: 0px;
  padding: 20px;
}
#form-content,
#form-content-1,
#form-content-2,
#form-content-3 {
  margin-top: 0;

  padding-top: 0;
  padding-bottom: 0;
}
#form-btn {
  background-color: #ff6f00;
  width: 100%;
}
#form-btn-2 {
  background-color: #ff6f00;
  width: 90%;
  margin-top: 0;
  padding-top: 0;
  margin-left: 20px;
}
.mx-auto {
  width: 90%;
  margin-top: 20px;
  padding-top: 0;
  margin-left: 20px;
}
#subsection {
  width: 100%;
}
#form-content-4 {
  padding: 0;
  margin-top: 0;
}
#headline-item {
  background-color: #1565c0;
}
.para-heading {
  color: white;
}
#first-para {
  text-align: center;
}
</style>
