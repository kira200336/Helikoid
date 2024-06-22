<script>
    import ContactForm from "$lib/components/ContactForm.svelte";

</script>

<svelte:head>
    <title>Helikoid | About Us</title>
    <meta property="og:site_name" content="About Helikoid"/>
    <meta name="description"
          content="Breath Life Into Your Systems With Cutting-edge AI Solutions">
    <meta property="og:title" content="Helikoid | About Us"/>
    <meta property="og:description"
          content="Breath Life Into Your Systems With Cutting-edge AI Solutions"/>
    <meta property="og:image" content="https://helikoid.ai/image.png">
    <meta property="og:url" content="https://helikoid.ai/about"/>
    <link rel="alternate" href="https://helikoid.ai" hreflang="en"/>
    <meta property="og:locale" content="en"/>
</svelte:head>

<div class="container">
    <div class="text-wrapper">
        <h1>Contact Us</h1>
    </div>
    <div class="features">
        <ContactForm/>
    </div>
</div>

<style lang="scss">

  .text-wrapper {
    margin-top: 160px;
    display: flex;
    flex-direction: column;
    box-sizing: border-box;

    p {
      margin-top: 10px;
    }

    h1 {
      margin: 0;
    }

    @media screen and (max-width: 568px) {
      margin-top: 60px;
    }

  }

  .features {
    margin: 40px auto;
    display: grid;
    grid-gap: 1rem;
    transition: 250ms ease-in-out all;
    grid-template-columns: repeat(3, 1fr);

    @media only screen and (max-width: 1000px) {
      grid-template-columns: repeat(2, 1fr);
    }

    @media only screen and (max-width: 680px) {
      grid-template-columns: repeat(1, 1fr);
    }

    div {
      padding: 1.25rem;
      border: 1px solid var(--card-border);
      background-color: var(--card-background);
      border-radius: 0.4rem;
      transition: 250ms ease-in-out all;
    }

    h2 {
      margin: 0;
      font-size: 1.25em;
    }
  }

</style>
