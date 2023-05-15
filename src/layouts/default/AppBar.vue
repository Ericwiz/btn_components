<template>
  <v-navigation-drawer
  color="grey-lighten-4"
  permanent
  >
    <v-list class="mb-12">
      <v-list-item>
        <span class="text-red">Dev</span>challenges.io
      </v-list-item>
    </v-list>

    <v-list>
        <v-list-item
        v-for="item in items"
        :key="item"
      >
      <router-link :to="item.url" 
      class="text-decoration-none text-grey-darken-1"
      >{{ item.label }}</router-link>
      </v-list-item>
    </v-list>
  </v-navigation-drawer>
</template>

<script>
  export default {
    data() {
      return {
        items: [
          {
            label: 'Color', url: '/colors'
          },
          {
            label: 'Typography', url: '/typography',
          },
          {
            label: 'Spaces', url: '/spaces'
          },
          {
            label: 'Buttons', url: '/'
          },
          {
            label: 'Inputs', url: '/inputs'
          },
          {
            label: 'Grids', url: '/grids'
          }
        ]
      }
    }
  }
</script>

<style scoped>
.active {
    /* color: #42b983; */
}

.exact-active-link {
    color: #000000;
    font-weight: bold;
}
</style>
