<!-- ButtonFromApp.svelte -->
<script>
  let className = '';
  export { className as class };
  export let success = false;
</script>

<button class="button-app m-4 {success ? 'bg-green-800' : ''} {className}"
  ><slot>Click me!</slot></button
>
