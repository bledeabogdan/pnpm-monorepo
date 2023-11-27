<svelte:head>
  <title>Home</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
  <pre>styles</pre>
  <h2 class="sui--single">
    try editing <strong>src/routes/+page.svelte</strong>
  </h2>
  <p>issue: not loading</p>

  <pre>@specialdoom/styles</pre>
  <h2 class="sui--single-2">
    try editing <strong>src/routes/+page.svelte</strong>
  </h2>
  <p>
    issue: loading, but error in file regarding that it's not finding the
    stylesheet
  </p>
</section>

<style lang="scss">
  @use "styles" as sty1;
  @use "@specialdoom/styles/scss/test" as sty2;

  section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    flex: 0.6;
  }

  h1 {
    width: 100%;
  }

  .welcome {
    display: block;
    position: relative;
    width: 100%;
    height: 0;
    padding: 0 0 calc(100% * 495 / 2048) 0;
  }

  .welcome img {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    display: block;
  }
</style>
