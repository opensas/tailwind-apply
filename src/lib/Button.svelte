<!-- CustomButton.svelte -->
<script>
  let className = '';
  export { className as class };
  export let success = false;
</script>

<button class="button {success ? 'bg-green-800' : ''} {className}"
  ><slot>Click me!</slot></button
>

<!-- This doesn't work either
<style lang="postcss">
  @tailwind components;
  @layer components {
    .button {
      @apply bg-blue-400 font-bold text-white rounded-lg p-4;
    }
  }
</style> -->

<style lang="postcss">
  .button {
    @apply bg-blue-400 font-bold text-white rounded-lg p-4;
  }
</style>
