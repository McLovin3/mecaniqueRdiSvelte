<script lang="ts">
	import FirstPage from "$lib/components/FirstPage.svelte";
	import SecondPage from "$lib/components/SecondPage.svelte";
	import { addMessages, getLocaleFromNavigator, init } from "svelte-i18n";
	import en from "$lib/translations/en.json";
	import fr from "$lib/translations/fr.json";
	import ThirdPage from "$lib/components/ThirdPage.svelte";
	import ContactUs from "$lib/components/ContactUs.svelte";

	addMessages("en", en);
	addMessages("fr", fr);

	init({
		fallbackLocale: "fr",
		initialLocale: getLocaleFromNavigator()
	});
</script>

<div class="h-screen l bg-[url('skytrak1.jpg')] bg-cover bg-center">
	<div class="bg-surface-600/[0.7] h-full snap-y snap-mandatory overflow-scroll">
		<div class="snap-center">
			<FirstPage />
		</div>
		<div class="snap-center">
			<SecondPage />
		</div>
		<div class="snap-center">
			<ThirdPage />
		</div>
		<div class="snap-center">
			<ContactUs />
		</div>
	</div>
</div>
