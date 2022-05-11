<script>
export default {
  props : {
    name : String,
    changeName: Function,
  },
   data () {
    return {
      dbName: this.name,
      detailName: "asdfsd",
    }
  },
}
</script>

<template>
  <h1>Detail</h1>
  <h1>{{ dbName }}</h1>
  <h1>{{detailName}}</h1>
  <input v-model="dbName" />
  <button @click="changeName(dbName)">click</button>
</template>
