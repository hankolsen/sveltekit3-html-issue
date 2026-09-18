# Issues with {@html} in SvelteKit 3

Trying to render invalid html using {@html} in SvelteKit 3 results in 500 error on the server.  
Two examples:

## Missing closing tag

```javascript
const text = '<p>Missing closing tag';

<div>{@html text}</div>
```

## html rendered inside the same tag

```javascript
const text = `<p>Valid html</p>`;

<p>{@html text}</p>
```
