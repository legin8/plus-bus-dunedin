<script>
  import RunDays from "./SupermarketDays.svelte";
</script>

<div>
  <h2>Days and Costs</h2>
  <p>We operate on Tuesdays and Thursdays.</p>
  <p>The cost depends on where you live in Dunedin.<br>$10-$14, return trip.</p>
  <p>This is based on the distance from your home to the supermarket and can be booked as a regular service or as a "one-off".</p>
  <div>
    <RunDays />
  </div>
</div>

<style>

</style>