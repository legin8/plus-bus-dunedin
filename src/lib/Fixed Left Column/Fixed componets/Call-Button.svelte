<script>
	import info from "../../site_info.json";
</script>

<div>
	<a href={info.contactNumberLink}>
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