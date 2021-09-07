<script>
  import Button from '$lib/Button.svelte';
  import ButtonFromApp from '$lib/ButtonFromApp.svelte';
</script>

<Button class="bg-indigo-500">Styles from component (overriding class - failed)</Button>
<ButtonFromApp class="bg-indigo-500">Styles from app.postcss (overriding class - ok)</ButtonFromApp>

<div class="w-full border my-2"/>

<Button sucess>Styles from component (custom prop - failed)</Button>
<ButtonFromApp success>Styles from app.postcss (custom prop - ok)</ButtonFromApp>
