<script>
  // This is divided into to columns, left and right.
  import LeftColumnLayout from "./lib/Fixed Left Column/Left-Column-Layout.svelte";
  import RightColumnLayout from "./lib/Scrolling Right Column/RightColumnLayout.svelte";
</script>

<!-- This is containing the layout of the left and right columns, when the screen is less than 930px
the left column is currently removed -->
<main>
  <div class="appLayoutMain">
    <div class="leftColumn">
      <LeftColumnLayout />
    </div>
    

    <div class="rightColumn">
      <RightColumnLayout />
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
