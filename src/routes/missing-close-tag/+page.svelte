<script lang="ts">
	const text = `<p>Missing closing tag`;
</script>

<h1>Missing close tag</h1>
<p>Reload the page to generate a 500 error</p>

<pre>
  <code>{text}</code>
</pre>

<h2>Issue</h2>
<!-- eslint-disable-next-line svelte/no-at-html-tags -->
<div class="html">{@html text}</div>

