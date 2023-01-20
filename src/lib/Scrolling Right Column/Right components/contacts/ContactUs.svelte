<script>
	import info from "../../../site_info.json";
</script>

<div>
	<h2>Contact us</h2>
	<div>
		<p>{info.plusBusDetails.displayPhoneNumber} (Co-ordinator)</p>
		<a href={info.plusBusDetails.emailLink}>
			<em>{info.plusBusDetails.email}</em>
		</a>
	</div>
	<div>
		<ul>
			{#each info.plusBusDetails.address as address}
				<li>{address}</li>
			{/each}
		</ul>
	</div>
</div>