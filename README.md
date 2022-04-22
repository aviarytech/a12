# a12

ui components

relies:

- svelte
- tailwind
- [iconify](https://icon-sets.iconify.design/)

## Install Dependencies

```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init tailwind.config.cjs -p
mv postcss.config.js postcss.config.cjs
```

## Install

```bash
npm install a12
```

## Configure Tailwind

```js
module.exports = {
	content: ['./src/**/*.{html,js,svelte,ts}', './node_modules/a12/**/*.{html,js,svelte,ts}'],
	theme: {
		extend: {}
	},
	plugins: []
};
```

## Use a12

```
<script>
	import { FeaturesGrid } from 'a12';
</script>

<FeaturesGrid
	subtitle="Deploy faster"
	title="Everything you need to deploy your app"
	description="Phasellus lorem quam molestie id quisque diam aenean nulla in. Accumsan in quis quis nunc, "
	features={[
		{
			title: 'Push to Deploy',
			description:
				'Ac tincidunt sapien vehicula erat auctor pellentesque rhoncus. Et magna sit morbi lobortis.',
			icon: 'heroicons-outline:cloud-upload'
		}
	]}
/>
```
