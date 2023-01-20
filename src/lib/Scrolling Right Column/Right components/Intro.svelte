<script>
  import info from "../../site_info.json";
</script>

<div class="intro">
  <div>
    <!-- This is the Heading and picture at the top of the page-->
    <h1 class="pageTitle">Plus Bus Dunedin</h1>
    <img src={info.assetAdresses.mainPicture} alt="Van">
  </div>
  
  <div>
    <h2>What we do</h2>
    <!-- The above is the subheading and the below is the information content, This is hard coded for now it may change -->
    <div>
      <ul class="introText">
        <li>At Plus Bus we provide a <span class="bold">"door-to-door service"</span></li>
        <li>Helping the <span class="italic">elderly and those that struggle using public transport</span> to get groceries home from the supermarket.</li>
        <li>Clients are picked up from their home in a van then,</li>
        <li>the van can carry up to nine passengers at a time.</li>
        <li>A volunteer helper will carry groceries back into your house.</li>
      </ul>
    </div>
  </div>
</div>


<style>
  /* This targets the main heading for the page */
  .intro h1 {
    font-size: 64px;
    margin: 20px auto;
  }

  /* This sets the size of the image under the heading */
  .intro img {
    width: 50vw;
    height: 30vw;
  }

  .intro .bold {
    font-weight: bold;
  }

  .intro .italic {
    font-style: italic;
  }
  
</style>