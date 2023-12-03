<script lang="ts">
	import { _ } from "svelte-i18n";

	let firstName = "";
	let lastName = "";
	let email = "";
	let subject = "";
	let formSubmitted = false;

	function onSubmit() {
		console.log("Form submitted");

		firstName = "";
		lastName = "";
		email = "";
		subject = "";
		formSubmitted = true;

		setTimeout(() => {
			formSubmitted = false;
		}, 5000);
	}
</script>

<section class="h-screen">
	<div class="flex flex-col justify-between h-full p-3">
		<div />
		<div
			class="w-2/3 mx-auto bg-surface-600 px-10 rounded-3xl justify-around flex flex-col py-7"
			style="height: 60%;"
		>
			<h2 class="text-6xl text-white text-center">{$_("contactUs.contactUs")}</h2>
			<form on:submit|preventDefault={onSubmit}>
				{#if formSubmitted}
					<div class="text-center text-white text-2xl mt-4">{$_("contactUs.messageSent")}</div>
				{:else}
					<div class="flex flex-row">
						<label class="label m-2 w-1/2" for="firstName">
							<span class="text-white text-2xl">{$_("contactUs.firstName")}</span>
							<input
								bind:value={firstName}
								required
								class="input"
								id="firstName"
								type="text"
								placeholder={$_("contactUs.firstName")}
							/>
						</label>
						<label class="label m-2 w-1/2" for="lastName">
							<span class="text-white text-2xl">{$_("contactUs.lastName")}</span>
							<input
								bind:value={lastName}
								required
								class="input"
								id="lastName"
								type="text"
								placeholder={$_("contactUs.lastName")}
							/>
						</label>
					</div>
					<label class="label m-2" for="email">
						<span class="text-white text-2xl">{$_("contactUs.email")}</span>
						<input
							bind:value={email}
							required
							class="input"
							id="email"
							type="email"
							placeholder={$_("contactUs.email")}
						/>
					</label>
					<label class="label m-2" for="subject">
						<span class="text-white text-2xl">{$_("contactUs.subject")}</span>
						<textarea
							bind:value={subject}
							required
							class="textarea"
							rows="4"
							placeholder={$_("contactUs.subject")}
						/>
					</label>
					<div class="text-end mt-4">
						<button class="btn variant-filled" type="submit">{$_("contactUs.submit")}</button>
					</div>
				{/if}
			</form>
		</div>
		<div class="flex flex-row justify-center text-white text-xl">
			<p>{$_("contactUs.phone")}: 450-922-2206</p>
			<div class="w-5" />
			<p>{$_("contactUs.address")}: Placeholder</p>
		</div>
	</div>
</section>
