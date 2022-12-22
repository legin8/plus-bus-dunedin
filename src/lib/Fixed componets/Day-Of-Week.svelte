<script>
	import { onMount } from "svelte";

	let dayOfWeek = "Error, no Day";
  let isRunning = "";
  const runDays = [2, 4];

	onMount(async function () {
    const date = new Date();
    let day = date.getDay();
    if (day == 0) dayOfWeek = "Sunday";
    if (day == 1) dayOfWeek = "Monday";
    if (day == 2) dayOfWeek = "Tuesday";
    if (day == 3) dayOfWeek = "Wednesday";
    if (day == 4) dayOfWeek = "Thursday";
    if (day == 5) dayOfWeek = "Friday";
    if (day == 6) dayOfWeek = "Saturday";

    ifRunning(day);
  });

  let ifRunning = day => {
    runDays.forEach(runningDay => {
      if (runningDay == day) isRunning = "is";
    });
    
    if (isRunning == "") isRunning = "isn't";
  }
</script>

<div class="thisDay">
  <div>It's {dayOfWeek} today</div>
  <div>The van {isRunning} running today</div>
</div>

<style>
  .thisDay {
    position: fixed;
    left: 10px;
    top: 10px;
    text-align: left;
    background-color: #f2b48c;
    border-radius: 20%;
    padding: 20px;
  }
</style>