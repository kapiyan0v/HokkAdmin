<template>
  <v-app dark>
    <v-navigation-drawer v-model="drawer" :clipped="clipped" app>
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar :clipped-left="clipped" fixed app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-toolbar-title v-text="title" />
      <v-spacer />
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer :absolute="!fixed">
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: true,
      drawer: false,
      fixed: false,
      title: 'Admin',
      items: [
        {
          title: 'Главная',
          to: '/',
        },
        {
          title: 'Перемещения',
          to: '/dislocation',
        },
        {
          title: 'Плановые маршруты',
          to: '/plan-routes',
        },
        {
          title: 'Плановые погрузки',
          to: '/plan-carriage',
        },
        {
          title: 'Плановые расписания',
          to: '/plan-schedule',
        },
        {
          title: 'Отчеты',
          to: '/report',
        },
        {
          title: 'Пути',
          to: '/routes',
        },
        {
          title: 'Станции',
          to: '/stations',
        },
        {
          title: 'Станции 2',
          to: '/stations2',
        },
        {
          title: 'Вагоны',
          to: '/vagons',
        },
      ],
    }
  },
}
</script>
