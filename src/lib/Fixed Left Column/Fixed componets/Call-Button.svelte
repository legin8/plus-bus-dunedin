<script>
	export let contactNumberLink;
</script>

<div>
	<a href={contactNumberLink}>
		<button class="callButton">Call</button>
	</a>
</div>

<style>
.callButton {
	margin: 20px;
  padding: 10px 20px;
  border-radius: 100%;
  font-weight: bold;
}
</style>