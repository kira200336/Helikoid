<script>
    import LinkArrow from "../icons/LinkArrow.svelte";
</script>

<div class="grid gap" id="community">
    <div class="row text">
        <h2>About Us</h2>
        <p>Our AI Automation Agency is your go-to partner for integrating AI and automation into your business, from initial conception to full-scale implementation and continuous support. We’re not just experts in AI and automation, we’re the team dedicated to transforming businesses into smarter, more efficient, and cutting-edge entities. Guided by our founder, Jamal Dahbi, we walk you through the entire transformation process, turning your vision into actionable, impactful solutions. With extensive expertise across various industries, we’ll help you craft an innovative strategy that not only optimizes efficiency but also accelerates growth, laying the groundwork for your company’s future success.</p>
    </div>
</div>

<style lang="scss">

  .grid {
    display: grid;
    grid-template-columns: repeat(12, minmax(0, 1fr));

    h2 {
      font-size: 3rem;

      @media screen and (max-width: 568px) {
        font-size: 2rem;
      }
    }
  }

  .gap {
    gap: 1rem;
  }

  .row {
    grid-column: span 12 / span 12;
  }

  .text {

    @media screen and (max-width: 1000px) {
      text-align: center;
    }

    h2 {
      font-size: 3rem;

      @media screen and (max-width: 568px) {
        font-size: 2rem;
      }
    }
  }

  .platform {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    background-color: var(--card-background);
    border: 1px solid var(--card-border);
    padding: 20px;
    grid-column: span 6 / span 6;
    text-decoration: none;
    border-radius: 5px;
    transition: 200ms ease-in-out;

    div {
      display: flex;
      justify-content: space-between;
    }

    h3, p {
      margin: 0;
    }

    @media screen and (max-width: 568px) {
      grid-column: span 12 / span 12;
    }

    &:hover {
      border-color: var(--success-color);
    }
  }

</style>
