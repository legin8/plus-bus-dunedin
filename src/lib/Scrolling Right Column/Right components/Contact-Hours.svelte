<script>
  import Hours from "./contacts/Hours.svelte";
  import Volunteer from "./contacts/Volunteer.svelte";
  import ContactUs from "./contacts/ContactUs.svelte";

  export let openHours;
  export let displayPhoneNumber;
</script>

<div>
  <Volunteer />
  <Hours {openHours} />
  <ContactUs {displayPhoneNumber} />
</div>
