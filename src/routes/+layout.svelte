<script lang="ts">
  import '#lib/style.css';

	const { children } = $props();
</script>

<div class="hero">
	{@render children?.()}
</div>
