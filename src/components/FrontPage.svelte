<script>
  import Category from "./Category.svelte";

  import TopNav from "./TopNav.svelte";
</script>

<div class="FrontPage">
  <TopNav />
  <div class="categorylist">
    <Category
      imgs={Array(14)
        .fill(0)
        .map((e, i) => i + 1)}
      title="De største sange lige nu"
    />
    <Category
      imgs={Array(14)
        .fill(0)
        .map((e, i) => i + 15)}
      title="Sleep"
    />
    <Category
      imgs={Array(14)
        .fill(0)
        .map((e, i) => i + 29)}
      title="Focus"
    />
  </div>
</div>

<style>
  .categorylist {
    padding: 1rem;
  }
</style>
