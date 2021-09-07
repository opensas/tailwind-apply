<script>
  import Button from '$lib/Button.svelte';
  import ButtonWithLayer from '$lib/ButtonWithLayer.svelte';
  import ButtonFromApp from '$lib/ButtonFromApp.svelte';
</script>

<h1>Using apply from a Svelte component and being able to override it</h1>

<h2>Overriding class via the class prop</h2>

<Button class="bg-indigo-500">Styles from component (FAILS!)</Button>
<ButtonWithLayer class="bg-indigo-500">Styles from component with layer (FAILS!)</ButtonWithLayer>
<ButtonFromApp class="bg-indigo-500">Styles from app.postcss (OK!)</ButtonFromApp>

<h2>Overriding class via a custom class</h2>

<Button sucess>Styles from component (FAILS!)</Button>
<ButtonWithLayer sucess>Styles from component (FAILS!)</ButtonWithLayer>
<ButtonFromApp success>Styles from app.postcss (OK!)</ButtonFromApp>
