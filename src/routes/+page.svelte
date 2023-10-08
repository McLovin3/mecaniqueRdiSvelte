<script lang="ts">
	let isFrench = true;

	function changeLanguage() {
		isFrench = !isFrench;
	}
</script>

<header class="h-screen bg-[url('skytrak1.jpg')] bg-cover bg-center">
	<div
		class="h-full bg-surface-500/[0.5] p-2 bg-[url('logo.png')] bg-[length:25%] bg-center bg-no-repeat"
	>
		<div class="flex flex-row">
			<p class="text-white underline text-3xl font-bold">450-922-2206</p>
			<div class="flex-grow" />
			<button class="btn variant-filled" on:click={changeLanguage}>
				{isFrench ? 'Anglais' : 'French'}
			</button>
		</div>
	</div>
</header>
