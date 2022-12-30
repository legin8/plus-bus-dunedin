<script>
  // Components imported here from the lib directory
  import LeftColumnLayout from "./lib/Fixed Left Column/Left-Column-Layout.svelte";

  import Intro from "./lib/Scrolling Right Column/Intro.svelte";
  import DaysCost from "./lib/Scrolling Right Column/Days-Cost.svelte";
  import ContactHours from "./lib/Scrolling Right Column/Contact-Hours.svelte";

  const openHours = ["8:30am", "2pm"];
  
</script>

<main>
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

  .appLayoutMain {
    display: grid;
    grid-template-columns: 280px 1fr;
  }

  .rightColumn {
    width: 70%;
    margin: auto;
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
