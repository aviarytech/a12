# a12

ui components

## Install

```bash
npm i a12
```

## Use

```
<script>
	import FeaturesGrid from 'a12/FeaturesGrid.svelte';
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
