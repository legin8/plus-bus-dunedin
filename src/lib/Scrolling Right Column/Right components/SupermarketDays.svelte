<script>
  // Array of objects that fill the list
  const table = [{day: "Tuesday Mornings", supermarket: "Countdown Mornington", area: "Mornington/Hill suburbs"},
  {day: "Thursday Mornings", supermarket: "Pak 'n' Save", area: "South Dunedin, Anderson's Bay and St Clair"},
  {day: "Thursday Afternoons", supermarket: "Countdown Andersons Bay", area: "South Dunedin, Anderson's Bay and Waverley"}];
  
  const newTable = {
    "days" : ["Tuesday Mornings", "Thursday Mornings", "Thursday Afternoons"],
    "supermarket" : ["Countdown Mornington", "Pak 'n' Save", "Countdown Andersons Bay"],
    "area" : [
      ["Mornington", "Hill suburbs"],
      ["South Dunedin", "Anderson's Bay", "St Clair"],
      ["South Dunedin", "Anderson's Bay", "Waverley"]
    ]
  }

</script>


<div>
  <ul class="runTable">
    {#each table as entry}
      <li>{entry.day}</li>
      <li>{entry.supermarket}</li>
      <li>{entry.area}</li>
    {/each}
  </ul>
  
</div>

<style>
  .runTable {
    display: grid;
    grid-template-columns: 2fr 2fr 1fr;
    font-weight: bold;
    text-align: left;
  }

  .runTable li {
    padding-top: 10px;
    padding-bottom: 10px;
  }

</style>