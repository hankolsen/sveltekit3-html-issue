<script lang="ts">
	const text = `<p>Valid html</p>`;
</script>

<h1>Valid html, but inside the same tag</h1>
<p>Reload the page to generate a 500 error</p>

<pre>
  <code>{text}</code>
</pre>

<h2>Issue</h2>
<!-- eslint-disable-next-line svelte/no-at-html-tags -->
<p class="html">{@html text}</p>

