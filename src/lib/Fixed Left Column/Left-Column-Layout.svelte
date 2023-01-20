<script>
	// Component imports
	import DayOfWeek from "./Fixed componets/Day-Of-Week.svelte";
	
	import CallButton from "./Fixed componets/Call-Button.svelte";
	import CallHover from "./Fixed componets/Call-Hover-Text.svelte"
	
  import EmailButton from "./Fixed componets/Email-Button.svelte";
  import EmailHoverText from "./Fixed componets/Email-Hover-Text.svelte";

	// variables to be passed, not used in this class
	export let openHours;
	export let contactNumberLink;
	export let displayPhoneNumber;

	let callButtonStatus = "hidText";
	let emailButtonStatus = "hidText";

	let callText = button => {
		resetHiddenText();
		if (button == "call") callButtonStatus = "showText";
		if (button == "email") emailButtonStatus = "showText";
	}
	
	let resetHiddenText = () => {
		callButtonStatus = "hidText";
		emailButtonStatus = "hidText";
	}

</script>

<div class="fixedComponents">
	<DayOfWeek />
	<div class="ButtonsBorder">
		<div class="sideContent">
			<h4 class="buttonHeadings">Inquiry and Booking</h4>

		<div class="callBookButtons">

			<!-- svelte-ignore a11y-mouse-events-have-key-events -->
			<div on:mouseover={() => callText("email")}>
				<EmailButton />
			</div>

			<!-- svelte-ignore a11y-mouse-events-have-key-events -->
			<div class="callButton" on:mouseover={() => callText("call")}>
				<CallButton {contactNumberLink} />
			</div>
		</div>

		<div class="{callButtonStatus}">
			<CallHover {openHours} {displayPhoneNumber} />
		</div>

		<div class="{emailButtonStatus}">
			<EmailHoverText />
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
		width: 250px;
	}

	.sideContent {
		margin-bottom: 20px;
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

	.hidText {
		display: none;
	}

	.showText {
		display: block;
	}

</style>