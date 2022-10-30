<template>
  <div component="NumeralIndex">
    <ul id="baseHeader">
      <li>Numerals</li>
      <li>About</li>
      <li>Operations</li>
      <li>Theory</li>
    <div id="content">
      <p>Введите свое число и систему счисления:</p>
      <input id="number">
      <p>в</p>
      <select id="numeralSelector">
        <option v-for="number of numbers" :key="number">{{number}}</option>
      </select>
      <select id="numeralSelector">
        <option v-for="number of numbers" :key="number">{{number}}</option>
      </select>
    </div>
  </ul>
</div>
</template>
<script>
export default {
  name: 'NumeralsIndex',
  el: '#numeralSelector',
  data () {
    return {
      numbers: ["2", "3", "4", "5", "6", "7", "8", "9", "10"],
      codes: ["Прямой код", "Обратный код", "Дополнительный код"]
    }
  }
}
</script>

<style scoped>
#
#baseHeader{
}
li #baseHeader{

}
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
