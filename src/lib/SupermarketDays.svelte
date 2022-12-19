<script>
  const table = [{day: "Tuesday Mornings", supermarket: "Countdown Mornington", area: "Mornington/Hill suburbs"},
{day: "Thursday Mornings", supermarket: "Pak 'n' Save", area: "South Dunedin, Anderson's Bay, St Clair"},
{day: "Thursday Afternoons", supermarket: "Countdown Andersons Bay", area: "South Dunedin, Anderson's Bay and Waverley"}];
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
    grid-template-columns: 1fr 1fr 1fr;
  }
</style>