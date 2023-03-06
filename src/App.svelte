<script>
  let name = "World"
  let src = "favicon.png"
  let count = 0

  const incrementCounter = () => {
    count += 1;
  }
</script>

<main>
  <h1>Hello {name}</h1>
  <h2>counter: {count}</h2>
  <button on:click={incrementCounter}>increment</button>
  <img src={src} alt="svelte" />
</main>

<style>

  main {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  h1 {
    font-size: 72px;
    text-align: center;
  }
</style>
