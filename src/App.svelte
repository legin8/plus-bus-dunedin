<script>
  // Components imported here from the lib directory
  import LeftColumnLayout from "./lib/Fixed Left Column/Left-Column-Layout.svelte";

  import Intro from "./lib/Intro.svelte";
  import DaysCost from "./lib/Days-Cost.svelte";
  import ContactHours from "./lib/Contact-Hours.svelte";

  const openHours = ["8:30am", "2pm"];
  
</script>

<main class="appMain">
  <div class="appLayoutMain">

    <div class="leftColumn">
      <LeftColumnLayout {openHours}/>
    </div>
    

    <div class="rightColumn">
      <div>
        <Intro />
      </div>
    
      <div>
        <DaysCost />
      </div>
    
      <div>
        <ContactHours {openHours} />
      </div>
    </div>
  
    
  
  </div>
  
</main>

<style>
  .appMain {
    width: 80vw;
  }

  .appLayoutMain {
    display: grid;
    grid-template-columns: 1fr 4fr;
    gap: 40px;
  }

  @media (max-width: 930px) {
    .leftColumn {
      display: none;
    }

    .appLayoutMain {
      display: block;
    }
  }

  

</style>
