<script>
	/**
	 * @type {any}
	 */
	export let a;
	/**
	 * @type {any}
	 */
	export let b;
	/**
	 * @type {any}
	 */
	export let url;
</script>

<div>
	<div class="w-[300px] h-[500px] relative">
        <div class=" absolute top-0 right-0 left-0 bottom-0 img-d h-[100%]" />

		<img alt="" src={url} class="w-[300px] h" />
		<div class="absolute top-0 p-2">
			<h1 class="text-[15px] font-[600]">{a}</h1>
			<p class="text-[20px] font-[500] ">{b}</p>
		</div>
	</div>
</div>
