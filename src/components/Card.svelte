<script>
  export let title;
  export let src;
  export let altText;
  export let aHref;
  export let desc;
</script>

<style>
  .selectionCards {
    display: inline-block;
    margin: 0 auto 50px;
    text-align: center;
    padding: 0 10px;
  }

  .v-mid {
    margin: auto;
    text-align: center;
  }

  .card-image {
    max-width: 250px;
  }
</style>

<div class="selectionCards">
  <article class="db dtc-ns tc w-100 w-50-ns ph3 v-mid">
    <div>
      <h1 class="card-title">{title}</h1>
    </div>
    <a href={aHref}>
      <img {src} class="card-image" alt={altText} />
    </a>
    <div class="pa3">
      <a href={aHref} class="link dim lh-title">{desc}</a>
    </div>
  </article>
</div>
