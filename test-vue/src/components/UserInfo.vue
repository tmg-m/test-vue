<script>
export default ({
  props : {
    name: {type: String},
    lastName: {type: String},
    city: {type: String},
    country: {type: String},
    continent: {type: String},
  }
})
</script>
<template>
  <h1>User Info</h1>
  <p>Name: {{name}}</p>
  <p>Last name: {{lastName}}</p>
  <p>City: {{city}}</p>
  <p>Country: {{country}}</p>
  <p>Continent: {{continent}}</p>
</template>