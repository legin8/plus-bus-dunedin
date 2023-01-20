<script>
	import info from "../../../site_info.json";
</script>

<div>
	<h2>Contact us</h2>
	<div>
		<p>{info.displayPhoneNumber} (Co-ordinator)</p>
		<a href={info.emailLink}>
			<em>{info.email}</em>
		</a>
	</div>
	<div>
		<ul>
			{#each info.address as address}
				<li>{address}</li>
			{/each}
		</ul>
	</div>
</div>