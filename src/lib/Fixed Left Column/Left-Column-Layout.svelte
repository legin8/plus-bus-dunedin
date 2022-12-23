<script>
	import DayOfWeek from "./Fixed componets/Day-Of-Week.svelte";
	import BookingDisplay from "./Fixed componets/Booking-Display.svelte";
</script>

<div class="fixedComponents">
	<DayOfWeek />
	<BookingDisplay />
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
	}
</style>