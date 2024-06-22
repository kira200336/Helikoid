<script>
    import Features from "$lib/components/landing/Features.svelte";
</script>

<svelte:head>
    <title>Helikoid | Services</title>
    <meta property="og:site_name" content="Helikoid"/>
    <meta name="description"
          content="Breath Life Into Your Systems With Cutting-edge AI Solutions">
    <meta property="og:title" content="Helikoid"/>
    <meta property="og:description"
          content="Breath Life Into Your Systems With Cutting-edge AI Solutions"/>
    <meta property="og:image" content="https://helikoid.ai/image.png">
    <meta property="og:url" content="https://helikoid.ai"/>
    <link rel="alternate" href="https://helikoid.ai" hreflang="en"/>
    <meta property="og:locale" content="en"/>
</svelte:head>

<div class="wrapper container">
    <h1>Our Services</h1>

    <Features/>
</div>

<style lang="scss">
  .wrapper {
    margin-top: 160px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    box-sizing: border-box;
    gap: 20px;

    h1 {
      margin: 0;
    }

    @media screen and (max-width: 568px) {
      margin-top: 60px;
    }
  }
</style>
