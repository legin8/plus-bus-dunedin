<script>
  import { onMount } from "svelte";
  let runDay = false;

  // This is for a future feature
  onMount(async function () {
    const date = await new Date();
    if (date.getDay() == 3 ) {
      runDay = true;
    }
    
    console.log(runDay);
    console.log(date.getDay());

  });


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
    padding: 0;
  }
</style>