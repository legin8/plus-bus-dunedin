<script>
  import Intro from "./lib/Intro.svelte";
  import DaysCost from "./lib/Days-Cost.svelte";
</script>

<main class="appMain">

  <div>
    <Intro />
  </div>

  <div>
    <DaysCost />
  </div>

</main>

<style>
  .appMain {
    width: 80vw;
  }
</style>
