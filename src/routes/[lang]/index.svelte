<script>
    import SignupNewsletter from "$lib/components/SignupNewsletter.svelte";
    import Hero from "$lib/components/landing/Hero.svelte";
    import Services from "$lib/components/landing/Services.svelte";
    import Blog from "$lib/components/landing/Blog.svelte";

</script>

<svelte:head>
    <title>Helikoid</title>
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

<div class="container flex">
    <div>
        <Hero/>
        <br>
        <Services/>
        <Blog/>  
    </div>
    <div>
        <SignupNewsletter/>
    </div>
</div>

<style lang="scss">

  .flex {
    display: flex;
    flex-direction: column;
    gap: 10rem;

    @media screen and (max-width: 568px){
      gap: 5rem;
    }
  }

</style>
