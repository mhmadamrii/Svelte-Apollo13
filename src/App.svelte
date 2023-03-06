<script>
  let name = "World"
  let src = "favicon.png"
  let count = 0

  const incrementCounter = () => {
    count += 1;
  }

  const handleInput = (event) => {
    name = event.target.value
  }

  console.log('rendered')
</script>

<main>
  <h1>Hello {name}</h1>
  <h2>counter: {count}</h2>
  <button on:click={incrementCounter}>increment</button>
  <input type="text" on:input={handleInput} bind:value={name} />
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
