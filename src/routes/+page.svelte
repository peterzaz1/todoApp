<script>
	let di;
</script>

<button
	on:click={() => di.showModal()}
	class="absolute bottom-5 right-5 bg-slate-700 text-white rounded-full p-4">open</button
>

<dialog bind:this={di} class="w-60 h-36 rounded-lg">
	<form class="flex flex-col justify-center items-center mt-6 gap-8">
		<input
			id="name"
			type="text"
			class="w-40 px-7 py-1 bg-slate-200 outline-none border-solid border-blue-900 border-2 rounded-md"
		/>
		<div class="flex items-stretch gap-4">
			<button class="bg-slate-700 py-2 px-4 rounded-md text-white">Add</button>
			<button
				class="bg-slate-700 py-2 px-4 rounded-md text-white"
				value="cancel"
				formmethod="dialog">Close</button
			>
		</div>
	</form>
</dialog>
