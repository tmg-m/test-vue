<script>
import UserInfo from '../components/UserInfo.vue';
import Detail from '../components/Detail.vue'
export default ({
  data() {
    return {
    userName: "Jon",
    userLastName: "Doe",
    userCity: "Barcelona",
    userCountry: "Spain",
    userContinent: "Europe",
    }
  },
  components : {
    UserInfo,
    Detail,
  },
  methods: {
    changeName (callName) {
      return this.userName= callName
    },
  },
})
</script>


<template>
  <h1>Home</h1>
  <div>
    <UserInfo :name="userName" :lastName="userLastName" :city="userCity" :country="userCountry" :continent="userContinent" />
  </div>
  <div>
    <Detail :name="userName" :changeName="changeName" />
  </div>
</template>