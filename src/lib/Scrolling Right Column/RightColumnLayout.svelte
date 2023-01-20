<script>
	import Intro from "./Right components/Intro.svelte";
  import DaysCost from "./Right components/Days-Cost.svelte";
  import ContactHours from "./Right components/Contact-Hours.svelte";

	export let openHours;
	export let displayPhoneNumber;

</script>

<div>
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

<style>

</style>