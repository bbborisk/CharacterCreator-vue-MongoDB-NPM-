<template>
  <div class="CharacterCreator">
    <h1>CharacterCreator</h1>
    <label for="character-name">Character name: </label>
    <input type="text" id="character-name" v-model="name" placeholder="Enter a name" />
    <br />
    <br />
      <label for="profession-list">Professions list: </label>
      <select id="profession-list" v-model="profession">
        <option value="Mage">Mage</option>
        <option value="Warrior">Warrior</option>
        <option value="Thief">Thief</option>
      </select>
      <p>{{name}}</p>
      <p>{{profession}}</p>
  </div>
</template>

<script>
export default {
  name: 'CharacterCreator',
  data: function(){
  return{
    name:"",
    profession: ""
  }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
