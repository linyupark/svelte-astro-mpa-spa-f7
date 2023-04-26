<script lang="ts">
  export let number = 0;
  const onAdd = () => {
    number++;
  };
</script>

<section>
  {number} <button on:click={onAdd}>+1</button>
</section>
