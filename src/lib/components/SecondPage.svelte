<script lang="ts">
	import { _ } from "svelte-i18n";
</script>

<section class="h-screen">
	<div class="flex flex-col justify-center h-full">
		<h2 class="text-8xl text-white text-center">{$_("secondPage.services")}</h2>
		<table class="w-1/2 mx-auto h-1/2 text-center text-white text-2xl m-3">
			<thead class="border-b-2">
				<tr>
					<th class="border-e-2">{$_("placeholder")}</th>
					<th class="border-s-2">{$_("placeholder")}</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<td class="border-e-2">{$_("placeholder")}</td>
					<td class="border-s-2">{$_("placeholder")}</td>
				</tr>
				<tr>
					<td class="border-e-2">{$_("placeholder")}</td>
					<td class="border-s-2">{$_("placeholder")}</td>
				</tr>
			</tbody>
		</table>
	</div>
</section>
