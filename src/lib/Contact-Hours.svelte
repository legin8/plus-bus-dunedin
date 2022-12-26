<script>
  import Hours from "./contacts/Hours.svelte";
  import Volunteer from "./contacts/Volunteer.svelte";
  import ContactUs from "./contacts/ContactUs.svelte";

  export let hours;
</script>

<div>
    <Volunteer />
    <Hours {hours} />
    <ContactUs />
</div>
