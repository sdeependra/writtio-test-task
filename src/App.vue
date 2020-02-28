<template>
  <div id="app">
    <writtio-dashboard />
  </div>
</template>

<script>

import WrittioDashboard from './components/WrittioDashboard';
export default {
  name: 'App',
  components:
  {
    WrittioDashboard
  },
  data()
  {
    return{
      chartData1 : [['NOV 15',300],['NOV 16',200],['NOV 17',420],['NOV 18',300],['NOV 19',200],['NOV 20',420],['NOV 21',200]],
      chartData2 : [['',15],['NOV 15',10],['',22],['',15],['NOV 19',10],['NOV 20',22],['NOV 21',10],['NOV 21',15],['NOV 21',10],['NOV 21',22],['NOV 21',15],['NOV 21',20],['NOV 21',22],['NOV 21',19],['NOV 21',15],['NOV 21',20],['NOV 21',22],['NOV 21',20],['NOV 21',22]],
      chartData3 : [['NOV 15',300],['NOV 16',200],['NOV 17',420],['NOV 18',300],['NOV 19',200],['NOV 20',420],['NOV 21',200]]
    }
  }
  
}
</script>

<style>
</style>
