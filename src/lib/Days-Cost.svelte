<script>
  // This imports a component to place under the content of this component
  import RunDays from "./SupermarketDays.svelte";
  const firstDays = "Tuesdays", secondDays = "Thursdays";
  const lowestFee = 10, highestFee = 14;
</script>

<div>
  <div class="dayCostInfo">
    <h2>Days and Costs</h2>
    <ul>
      <li>We operate on <strong>{firstDays}</strong> and <strong>{secondDays}</strong>,</li>
      <li>The cost depends on where you live in <i>Dunedin.</i></li>
      <li>${lowestFee}-${highestFee}, return trip.</li>
      <li>This is based on the distance from your <i>home</i> to the <i>supermarket.</i></li>
      <li>It can be booked as a <i>regular</i> or as a <i>"one-off" service</i>.</li>
    </ul>
  </div>
  
  <div>
    <RunDays />
  </div>
</div>

<style>
  .dayCostInfo {
    margin: 50px auto;
  }

  
</style>