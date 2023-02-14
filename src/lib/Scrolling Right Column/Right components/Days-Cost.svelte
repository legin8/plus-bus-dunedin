<script>
  import info from "../../site_info.json";
  // This imports a component to place under the content of this component
  import RunDays from "./SupermarketDays.svelte";
</script>

<div>
  <div class="dayCostInfo">
    <h2>Days and Costs</h2>
    <ul>
      <li>We operate on <strong>{info.plusBusDetails.officeDays[0]}</strong> and <strong>{info.plusBusDetails.officeDays[1]}</strong>,</li>
      <li>The cost depends on where you live in <i>Dunedin.</i></li>
      <li>${info.plusBusDetails.feeRange[0]} - ${info.plusBusDetails.feeRange[1]}, return trip.</li>
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