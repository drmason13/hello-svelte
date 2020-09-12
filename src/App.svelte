<script>
	// shoelace: import assets and components and register them
	import '@shoelace-style/shoelace/dist/shoelace/shoelace.css';
	import { defineCustomElements, setAssetPath } from '@shoelace-style/shoelace/dist/custom-elements';

	setAssetPath(document.currentScript.src);
	defineCustomElements();
	// end shoelace

	export let name;
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <sl-button type="primary" href="https://svelte.dev/tutorial">Svelte tutorial</sl-button> to learn how to build Svelte apps.</p>
	<sl-rating></sl-rating>
	<br>
	<sl-color-picker inline></sl-color-picker>
	<br>
	<sl-dropdown placement="top-start">
		<sl-button slot="trigger" caret>Edit</sl-button>
		<sl-menu>
			<sl-menu-item>Cut</sl-menu-item>
			<sl-menu-item>Copy</sl-menu-item>
			<sl-menu-item>Paste</sl-menu-item>
			<sl-menu-divider></sl-menu-divider>
			<sl-menu-item>Find</sl-menu-item>
			<sl-menu-item>Replace</sl-menu-item>
		</sl-menu>
	</sl-dropdown>
</main>

<style>
</style>