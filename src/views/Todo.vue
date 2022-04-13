<template>
  <div class="home">
    <v-list
      flat
    >
        <v-list-item>
          <template v-slot:default="{ active, }">
            <v-list-item-action>
              <v-checkbox
                :input-value="active"
                color="primary"
              ></v-checkbox>
            </v-list-item-action>

            <v-list-item-content>
              <v-list-item-title>Wake up</v-list-item-title>
              
            </v-list-item-content>
          </template>
        </v-list-item>
    </v-list>
  </div>
</template>

<script>
  

  export default {
    name: 'Home',
    data() {
      return {
        tasks: [
        {
          id: 1,
          title: 'wake up'
        },
          {
          id: 2,
          title: 'eat Lunch'
        },
          {
          id: 3,
          title: 'whatch tv'
        },
      ]
      }
      
    }

  
  }
</script>
