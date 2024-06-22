<script>
    import Team from "../../../lib/components/teams/Teams.svelte";
</script>

<svelte:head>
    <title>Helikoid | Team</title>
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
    <h1>Teams</h1>
    <Team/>
</div>

<style lang="scss">

  .wrapper {
    margin-top: 160px;
    margin-bottom: 40px;
    box-sizing: border-box;

    @media screen and (max-width: 568px) {
      margin-top: 60px;
    }
  }

  .text-wrapper {
    margin-bottom: 60px;
  }

  .tools {
    display: flex;
    gap: 1rem;
    margin: 4rem 0;

    @media only screen and (max-width: 1000px) {
      flex-direction: column;
    }
  }

</style>
