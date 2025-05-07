<script>
  let count = 0;

  function increment() {
    count += 1;
  }

  function decrement() {
    count -= 1;
  }

  function reset() {
    count = 0;
  }
</script>

<main>
  <h1>Contador con Svelte</h1>
  <h2>{count}</h2>
  <button on:click={increment}>Incrementar</button>
  <button on:click={decrement}>Disminuir</button>
  <button on:click={reset}>Reiniciar</button>
</main>

<style>
  main {
    text-align: center;
    padding: 2rem;
    font-family: sans-serif;
  }

  button {
    margin: 0.5rem;
    padding: 0.5rem 1rem;
    font-size: 1rem;
  }
</style>
