<template>
  <div class="main">
    <h1>Главная страница</h1>
    <v-row>
      <v-col>
        <nuxt-link to="/dislocation">
          <v-card class="main_inner_card">
            <h2>Перемещения</h2>
            <p>Перемещения</p>
          </v-card>
        </nuxt-link>
      </v-col>
      <v-col>
        <nuxt-link to="/plan-routes">
          <v-card class="main_inner_card">
            <h2>Плановые маршруты</h2>
            <p>Плановые маршруты</p>
          </v-card>
        </nuxt-link>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <nuxt-link to="/plan-carriage">
          <v-card class="main_inner_card">
            <h2>Плановые погрузки</h2>
            <p>Плановые погрузки</p>
          </v-card>
        </nuxt-link>
      </v-col>
      <v-col>
        <nuxt-link to="/plan-schedule">
          <v-card class="main_inner_card">
            <h2>Плановые расписания</h2>
            <p>Плановые расписания</p>
          </v-card>
        </nuxt-link>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <nuxt-link to="/report">
          <v-card class="main_inner_card">
            <h2>Отчеты</h2>
            <p>Отчеты</p>
          </v-card>
        </nuxt-link>
      </v-col>
      <v-col>
        <nuxt-link to="/routes">
          <v-card class="main_inner_card">
            <h2>Пути</h2>
            <p>Пути</p>
          </v-card>
        </nuxt-link>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <nuxt-link to="/stations">
          <v-card class="main_inner_card">
            <h2>Станции</h2>
            <p>Станции</p>
          </v-card>
        </nuxt-link>
      </v-col>
      <v-col>
        <nuxt-link to="/stations2">
          <v-card class="main_inner_card">
            <h2>Станции 2</h2>
            <p>Станции 2</p>
          </v-card>
        </nuxt-link>
      </v-col>
      <v-col>
        <nuxt-link to="/vagons">
          <v-card class="main_inner_card">
            <h2>Вагоны</h2>
            <p>Вагоны</p>
          </v-card>
        </nuxt-link>
      </v-col>
    </v-row>
  </div>
</template>

<style lang="scss">
.main {
  padding: 20px;
  font-size: 16px;
  h1 {
    margin-bottom: 40px;
  }
  a {
    text-decoration: none;
  }
  &_inner {
    &_card {
      padding: 20px 40px;
      h2 {
        font-size: 28px;
      }
      &:hover {
        background-color: #ffe328;
        color: #333;
        transition: 0.4s ease;
      }
    }
  }
}
</style>