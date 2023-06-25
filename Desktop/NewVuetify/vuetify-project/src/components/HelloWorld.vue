<template>
  <v-container class="fill-height">
    <v-responsive class="align-center text-center fill-height">
      
      <v-card>
        <v-tabs v-model="tab" color="deep-purple-accent-4" align-tabs="center">
          <v-tab :value="1">Landscape</v-tab>
          <v-tab :value="2">City</v-tab>
          <v-tab :value="3">Abstract</v-tab>
        </v-tabs>
        <v-window v-model="tab">
          <v-window-item v-for="n in 3" :key="n" :value="n">
            <v-container fluid>
              <v-row>
                <v-col v-for="i in 6" :key="i" md="4">
                  <v-img :src="`https://picsum.photos/500/300?image=${i * n * 5 + 10}`"
                    :lazy-src="`https://picsum.photos/10/6?image=${i * n * 5 + 10}`" aspect-ratio="1"></v-img>
                </v-col>
              </v-row>
            </v-container>
          </v-window-item>
        </v-window>
      </v-card>
      <v-expansion-panels variant="popout" class="my-4">
        <v-expansion-panel v-for="i in 5" :key="i" title="Item"
          text="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."></v-expansion-panel>
      </v-expansion-panels>
      <v-timeline>
        <v-timeline-item dot-color="purple-lighten-2" fill-dot>
          <v-card>
            <v-card-title class="bg-purple-lighten-2">
              <v-icon size="large" class="me-4" icon="mdi-magnify"></v-icon>
              <h2 class="font-weight-light">
                Title 1
              </h2>
            </v-card-title>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
          </v-card>
        </v-timeline-item>

        <v-timeline-item dot-color="amber-lighten-1" fill-dot size="x-small">
          <v-card>
            <v-card-title class="bg-amber-lighten-1 justify-end">
              <h2 class="me-4 font-weight-light">
                Title 2
              </h2>
              <v-icon size="large" icon="mdi-home-outline"></v-icon>
            </v-card-title>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
          </v-card>
        </v-timeline-item>

        <v-timeline-item dot-color="cyan-lighten-1" fill-dot>
          <v-card>
            <v-card-title class="bg-cyan-lighten-1">
              <v-icon class="me-4" size="large" icon="mdi-email-outline"></v-icon>
              <h2 class="font-weight-light">
                Title 3
              </h2>
            </v-card-title>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
          </v-card>
        </v-timeline-item>

        <v-timeline-item dot-color="red-lighten-1" fill-dot size="x-small">
          <v-card>
            <v-card-title class="bg-red-lighten-1 justify-end">
              <h2 class="me-4 font-weight-light">
                Title 4
              </h2>
              <v-icon size="large" icon="mdi-account-multiple-outline"></v-icon>
            </v-card-title>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
          </v-card>
        </v-timeline-item>

        <v-timeline-item dot-color="green-lighten-1" fill-dot>
          <v-card>
            <v-card-title class="bg-green-lighten-1">
              <v-icon class="me-4" size="large" icon="mdi-phone-in-talk"></v-icon>
              <h2 class="font-weight-light">
                Title 5
              </h2>
            </v-card-title>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>
            <v-card-text>
              Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod
              convenire principes at. Est et nobis iisque percipit.
            </v-card-text>

          </v-card>
        </v-timeline-item>
      </v-timeline>
      

    </v-responsive>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    tab: null,
  }),
}
</script>
