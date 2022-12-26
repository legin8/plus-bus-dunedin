<script>
	// Component imports
	import DayOfWeek from "./Fixed componets/Day-Of-Week.svelte";
	import BookingDisplay from "./Fixed componets/Email-Button.svelte";
	import CallButton from "./Fixed componets/Call-Button.svelte";

</script>

<div class="fixedComponents">
	<DayOfWeek />
	<div>
		<div class="ButtonsBorder">
			<h4 class="buttonHeadings">Inquiry and Booking</h4>

			<div class="callBookButtons">	
			<BookingDisplay />
			<CallButton />
			</div>
		</div>
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
		text-align: left;
	}

	.ButtonsBorder {
		border: #333 3px solid;
		border-radius: 19%;
		margin-top: 20px;
	}

	.buttonHeadings {
		position: relative;
		margin: 0px;
		top: 10px;
		text-align: center;
	}

	.callBookButtons {
		display: flex;
		justify-content: space-around;
		padding-top: 10px;
	}
</style>