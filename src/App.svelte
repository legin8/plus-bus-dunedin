<script>
  // Components imported here from the lib directory
  import Intro from "./lib/Intro.svelte";
  import DaysCost from "./lib/Days-Cost.svelte";
  import ContactHours from "./lib/Contact-Hours.svelte";
</script>

<main class="appMain">
  <div>
    <Intro />
  </div>

  <div>
    <DaysCost />
  </div>

  <div>
    <ContactHours />
  </div>

</main>

<style>
  .appMain {
    width: 80vw;
  }
</style>
