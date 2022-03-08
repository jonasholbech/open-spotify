<script>
  import Album from "./Album.svelte";
  export let imgs;
  export let title;
</script>

<article>
  <header>
    <h2>{title}</h2>
    <a href="#/seeall">See all</a>
  </header>
  <section class="albums">
    {#each imgs as img}
      <Album {img} />
    {/each}
  </section>
</article>

<style>
  article {
    margin-bottom: 2rem;
    overflow: hidden;
  }
  h2 {
    margin: 0;
  }
  header {
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    margin-bottom: 1rem;
  }
  .albums {
    display: flex;
    max-width: calc(100vw - 250px);
    overflow-x: auto;
    gap: 1rem;
  }
</style>
