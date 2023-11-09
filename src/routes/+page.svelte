<script lang="ts">
	let isFrench = true;

	function changeLanguage() {
		isFrench = !isFrench;
	}
</script>

<header class="h-screen bg-[url('skytrak1.jpg')] bg-cover bg-center">
	<div class="bg-surface-500/[0.5] h-full">
		<div class="flex flex-col justify-between h-full p-3">
			<div class="flex flex-row">
				<p class="text-white underline text-3xl font-bold">450-922-2206</p>
				<div class="flex-grow" />
				<button class="btn variant-filled" on:click={changeLanguage}>
					{isFrench ? 'Anglais' : 'French'}
				</button>
			</div>
			<div class="flex flex-col">
				<img class="max-w-lg m-auto" alt="RDI Logo" src="logo.png" />
				<h1 class="text-4xl font-bold text-center text-white">
					<span class="rdi-blue">R</span>éparation | <span class="rdi-blue">D</span>iagnostique |
					<span class="rdi-blue">I</span>nspection
				</h1>
			</div>
			<div>
				<p class="text-white text-center text-2xl font-bold mb-3">Nous réparons</p>
				<div class="grid grid-cols-8 divide-x w-2/3 mx-auto">
					<div class="flex justify-center items center">
						<img class="w-28 h-12" src="skyjack-logo.svg" alt="Skyjack Logo" />
					</div>
					<div class="flex justify-center items center">
						<img class="w-28 h-12" src="genie-logo.png" alt="Genie Logo" />
					</div>
					<div class="flex justify-center items center">
						<img class="w-28 h-12" src="imer-logo.png" alt="Imer Logo" />
					</div>
					<div class="flex justify-center items center">
						<img class="w-28 h-12" src="jlg-logo.png" alt="JLG Logo" />
					</div>
					<div class="flex justify-center items center">
						<img class="w-28 h-12" src="skytrak-logo.png" alt="Skytrak Logo" />
					</div>
					<div class="flex justify-center items center">
						<img class="w-28 h-12" src="volvo-logo.svg" alt="Volvo Logo" />
					</div>
					<div class="flex justify-center items center">
						<img class="w-28 h-12" src="cat-logo.png" alt="Cat Logo" />
					</div>
					<div class="flex justify-center items center">
						<img class="w-28 h-12" src="jd-logo.png" alt="JD Logo" />
					</div>
				</div>
			</div>
		</div>
	</div>
</header>
