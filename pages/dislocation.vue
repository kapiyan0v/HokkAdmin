<template>
  <div class="dislocations">
    <v-row>
      <h1 class="title">Перемещения</h1>
    </v-row>
    <v-row>
      <v-data-table
        single-select
        :headers="headers"
        :items="dislocations"
        :search="search"
        show-select
        class="table"
      >
        <template v-slot:top>
          <v-text-field
            v-model="search"
            label="Поиск перемещений"
            class="mx-4 pt-6"
            outlined
            prepend-icon="mdi-magnify"
            clearable
          ></v-text-field>
        </template>
      </v-data-table>
    </v-row>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
.dislocations {
  background-color: #0a0a0a;
  padding: 40px;
  border-radius: 5px;
  .title {
    margin-bottom: 40px;
  }
  &_search {
    margin-top: 30px;
  }
  .export {
    display: flex;
    justify-content: flex-end;
  }
  .table {
    margin-bottom: 20px;
  }
}
</style>