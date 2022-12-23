<script>
	import DayOfWeek from "./Fixed componets/Day-Of-Week.svelte";
	import BookingDisplay from "./Fixed componets/Booking-Display.svelte";
	import CallButton from "./Fixed componets/Call-Button.svelte";
</script>

<div class="fixedComponents">
	<DayOfWeek />
	<div class="callBookButtons">
		<BookingDisplay />
		<CallButton />
	</div>
	
	
</div>

<style>
	.fixedComponents {
		position: fixed;
		left: 10px;
		top: 20px;
		padding: 20px;
		background-color: #f2b48c;
		border-radius: 20%;
		margin: auto;
		text-align: left;
	}

	.callBookButtons {
		display: flex;
	}
</style>