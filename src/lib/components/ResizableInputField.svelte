<script lang="ts">
	export let value: string;
	export let mono: boolean = false;
</script>

<textarea
	class="w-full h-40 min-h-11 px-3 py-2 rounded-lg {mono ? 'font-mono' : 'font-sans'}
	bg-gray-900 text-slate-300 placeholder-slate-400
    valid:focus:ring-green-400 invalid:ring-red-500 focus:ring-2 focus:outline-none
    border border-slate-500 border-opacity-0 hover:border-opacity-100 focus:border-opacity-0"
	bind:value
	{...$$restProps}
	on:change
/>
