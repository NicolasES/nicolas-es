<template>
  <v-app>
    <v-app-bar>
      <v-container>
        <v-row>
          <v-col>
            <v-app-bar-title>
              <span>
                <v-icon color="blue-darken-2">mdi-store</v-icon>
                MY-COMPANY
              </span>
            </v-app-bar-title>


          </v-col>

          <v-spacer></v-spacer>
          <v-col class="d-flex flex-grow-0">
            <v-btn color="deep-purple-lighten-2" variant="text">
              Reserve
            </v-btn>
            <v-btn color="deep-purple-lighten-2" variant="text">
              Reserve
            </v-btn>
            <v-btn color="deep-purple-lighten-2" variant="text">
              Reserve
            </v-btn>
          </v-col>
        </v-row>
      </v-container>
    </v-app-bar>

    <!-- main content -->
    <v-main>
      <!-- 
        <v-parallax
        src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
      > -->

      <!-- presentation -->
      <section>
        <v-container>
          <v-row align="center" justify="space-between">
            <v-col cols="5">

              <h1 class="">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              </h1>
              <p class="my-4 text-subtitle-1">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mollis eu
                nibh non pretium.</p>
              <v-btn color="primary" size="x-large">GET START</v-btn>
            </v-col>

            <v-col cols="6">
              <v-img src="https://placehold.co/500x500" cover width="500" class="ml-auto"></v-img>
            </v-col>
          </v-row>
        </v-container>
      </section>

      <!-- services -->
      <section class="bg-light-blue-lighten-4">
        <v-container>
          <v-row justify="center">
            <v-col cols="6">
              <h2 class="text-center">Our services!</h2>
              <p class="text-center text-subtitle-1 font-weight-thin">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
                dolore magna aliqua.
              </p>
            </v-col>
          </v-row>

          <v-row justify="center" align="center">
            <v-col v-for="n in 4">
              <v-card class="mx-auto" max-width="400">
                <!-- <template v-slot:image>
                    <v-img class="align-end text-white" height="200"
                    src="https://cdn.vuetifyjs.com/images/cards/docks.jpg" cover>
                  </v-img>
                </template> -->
                <div class="d-flex justify-center">
                  <v-icon color="blue-darken-2" size="50" class="my-15">mdi-account-group</v-icon>
                </div>

                <v-card-title class="text-center font-weight-bold">Lorem ipsum dolor</v-card-title>

                <v-card-text class="text-center">
                  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
                    labore et dolore magna aliqua.</p>
                </v-card-text>

                <v-card-actions class="justify-center">
                  <v-btn color="deep-purple-lighten-2" variant="text">
                    Reserve
                  </v-btn>
                </v-card-actions>
              </v-card>

            </v-col>
          </v-row>
        </v-container>
      </section>


      <!-- gallery -->
      <section>
        <v-container>
          <v-row justify="center">
            <v-col cols="6">
              <h2 class="text-center">gallery!</h2>
              <p class="text-center text-subtitle-1 font-weight-thin">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
                dolore magna aliqua.
              </p>
            </v-col>
          </v-row>

          <v-row>
            <v-col cols="4" v-for="n in 9">
              <v-img :src="`https://picsum.photos/500/300?image=${n * 5 + 20}`"
                :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 20}`" cover />
            </v-col>
          </v-row>
        </v-container>
      </section>


      <!-- </v-parallax> -->
    </v-main>

    <v-footer class="bg-light-blue-lighten-4">
      <v-container>
        <v-row>
          <v-col cols="3">
            <div>
              <h3>Addres</h3>
              <span class="text-medium-emphasis">
                1234 Elm Street Anytown, USA 12345
              </span>
            </div>
          </v-col>
          <v-col cols="3">
            <div>
              <h3>Phone</h3>
              <span class="text-medium-emphasis">
                Reception: +212 555 1234 <br />
                Office: +214 789 5678
              </span>
            </div>
          </v-col>
          <v-col cols="3">
            <div>
              <h3>Email</h3>
              <span class="text-medium-emphasis">
                Office : fake@email.com <br />
              </span>
            </div>
          </v-col>
          <v-col cols="3">
            <div>
              <h3>Social</h3>
              <v-btn class="mx-2" icon="mdi-facebook" variant="text"></v-btn>
              <v-btn class="mx-2" icon="mdi-twitter" variant="text"></v-btn>
              <v-btn class="mx-2" icon="mdi-linkedin" variant="text"></v-btn>
              <v-btn class="mx-2" icon="mdi-instagram" variant="text"></v-btn>
            </div>
          </v-col>
        </v-row>

        <v-row>
          <v-col class="text-center">
            © All Rights Reserved by my-company.com
          </v-col>
        </v-row>
      </v-container>
    </v-footer>
  </v-app>
</template>

<script setup>
</script>

<style>
html {
  font-family: inherit !important;
}

section:first-child {
  margin-top: 50px;
}

section {
  margin-bottom: 100px;
  padding: 30px 0;
}

h1 {
  font-family: Roboto, sans-serif !important;
  font-size: 2.5rem !important;
}

h2 {
  font-family: Roboto, sans-serif !important;
  font-size: 2rem !important;
}</style>