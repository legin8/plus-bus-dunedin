<script>
  // This is divided into to columns, left and right.
  import LeftColumnLayout from "./lib/Fixed Left Column/Left-Column-Layout.svelte";
  import RightColumnLayout from "./lib/Scrolling Right Column/RightColumnLayout.svelte";


  // These variables are set up so you change them here and only here
  const openHours = ["8:30am", "2pm"]; // expects an array, with a start and finish only
  const contactNumberLink = "tel:+6434554050"; // expects a string, never change the tel:+64 part
  const displayPhoneNumber = "03 455 4050";
</script>

<!-- This is containing the layout of the left and right columns, when the screen is less than 930px
the left column is currently removed -->
<main>
  <div class="appLayoutMain">
    <div class="leftColumn">
      <LeftColumnLayout {openHours} {contactNumberLink} {displayPhoneNumber} />
    </div>
    

    <div class="rightColumn">
      <RightColumnLayout {openHours} {displayPhoneNumber} />
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


  /* break points */
  @media (max-width: 930px) {
    .leftColumn {
      display: none;
    }

    .appLayoutMain {
      display: block;
    }
  }

  

</style>
