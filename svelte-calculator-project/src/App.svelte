<script>
  import CalculatorButton from "./components/CalculatorButton.svelte";
</script>

<div class="container">
  {#each Array(9) as _, i}
    <CalculatorButton name={i + 1} />
  {/each}
  <!-- {#each <CalculatorButton name=1/>} -->
</div>

<style>
  .container {
    display: grid;
    background-color: #8ca0ff;
    width: 100%;
    grid-auto-rows: 50px;
    grid-template-columns: repeat(3, 1fr);
    column-gap: 20px;
  }
</style>
