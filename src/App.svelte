<script>
  // Components imported here from the lib directory
  import LeftColumnLayout from "./lib/Fixed Left Column/Left-Column-Layout.svelte";

  import Intro from "./lib/Scrolling Right Column/Intro.svelte";
  import DaysCost from "./lib/Scrolling Right Column/Days-Cost.svelte";
  import ContactHours from "./lib/Scrolling Right Column/Contact-Hours.svelte";

  // These variables are set up so you change them here and only here
  const openHours = ["8:30am", "2pm"]; // expects an array, with a start and finish only
  const contactNumberLink = "tel:+6434554050"; // expects a string, never change the tel:+64 part, this is used for a href
  const displayPhoneNumber = "03 455 4050";

  
</script>

<main>
  <div class="appLayoutMain">

    <div class="leftColumn">
      <LeftColumnLayout {openHours} {contactNumberLink} {displayPhoneNumber} />
    </div>
    

    <div class="rightColumn">
      <div>
        <Intro />
      </div>
    
      <div>
        <DaysCost />
      </div>
    
      <div>
        <ContactHours {openHours} {displayPhoneNumber} />
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
