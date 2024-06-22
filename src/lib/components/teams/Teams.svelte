<script>
    //Feature texts
    import {LL, locale} from "$i18n/i18n-svelte";

    const features = [
        {
            src: "",
            title: "Josh Brown",
            text: "Co-Founder",
            linkedin: "https://www.linkedin.com/in/liamottley/"
        },
        {
            src: "",
            title: "Liam Ottley",
            text: "Co-Founder",
            linkedin: "https://www.linkedin.com/in/liamottley/"
        }
    ]
</script>

<div class="features">
    {#each features as card}
        <div class="layered-shadow">
            <img src="{card.src}">
            <h2>{card.title}</h2>
            <p>{card.text}</p>
            <a href={card.linkedin} target="_blank" class="w-inline-block"><div class="w-embed"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M12 0C5.37258 0 0 5.37258 0 12C0 18.6274 5.37258 24 12 24C18.6274 24 24 18.6274 24 12C24 5.37258 18.6274 0 12 0ZM5.76172 9.93896H8.48118V18.1098H5.76172V9.93896ZM8.65899 7.41135C8.64134 6.6102 8.06844 6 7.13813 6C6.20781 6 5.59961 6.6102 5.59961 7.41135C5.59961 8.1959 6.18984 8.82367 7.10282 8.82367H7.1202C8.06844 8.82367 8.65899 8.1959 8.65899 7.41135ZM15.1554 9.74721C16.9449 9.74721 18.2865 10.9153 18.2865 13.425L18.2864 18.1099H15.5671V13.7385C15.5671 12.6405 15.1735 11.8913 14.1891 11.8913C13.4378 11.8913 12.9903 12.3964 12.7937 12.8842C12.7218 13.0591 12.7042 13.3027 12.7042 13.5469V18.1101H9.98438C9.98438 18.1101 10.0202 10.706 9.98438 9.93929H12.7042V11.0966C13.0651 10.5403 13.7115 9.74721 15.1554 9.74721Z" fill="black"></path>
</svg></div></a>
        </div>
    {/each}
</div>

<style lang="scss">
  .features {
    margin: 1rem 0;
    display: grid;
    grid-gap: 1rem;
    transition: 250ms ease-in-out all;
    grid-template-columns: repeat(12, minmax(0, 1fr));


    div {
      grid-column: span 6 / span 6;
      padding: 1.25rem;
      min-height: 200px;
      border: 1px solid var(--card-border);
      background-color: var(--card-background);
      border-radius: 0.4rem;
      transition: 250ms ease-in-out all;

      @media only screen and (max-width: 1000px) {
        grid-column: span 6 / span 6;
      }

      @media only screen and (max-width: 680px) {
        grid-column: span 12 / span 12;
        min-height: 180px;
      }
    }

    p {
      margin-top: 5px;
    }

    h2 {
      margin: 0;
      font-size: 1.25em;
    }
  }
</style>
