<script>
    import {locale, LL} from "$i18n/i18n-svelte";
    import LinkArrow from "../icons/LinkArrow.svelte";
</script>

<div class="grid gap" id="community">
    <div class="row text">
        <h2>Blog</h2>
        <p>Explore the most recent advancements in AI development, as shared by our industry leading engineers.</p>
    </div>
    <div class="row grid gap">
        <a class="platform layered-shadow" href="/{$locale}/blog/introducing_agentive">
            <div>
                <h3>Introducing Agentive</h3>
                <LinkArrow/>
            </div>
            <p>Explore Agentive: Streamlining the Creation, Management, and Deployment of Advanced AI Agents</p>
        </a>
        <a class="platform layered-shadow" href="/{$locale}/blog/an_inside_look_into_our_team">
            <div>
                <h3>An Inside Look Into Our Team</h3>
                <LinkArrow/>
            </div>
            <p>Meet the team behind Helikoid AI and learn more about how we are cultivating a culture of innovation and collaboration.</p>
        </a>
        <a class="platform layered-shadow" href="/{$locale}/blog/what_openai_devday_announcements_mean_for_your_business">
            <div>
                <h3>What OpenAI's Devday Announcements Mean For Your Business.</h3>
                <LinkArrow/>
            </div>
            <p>A Discussion with Helikoid's CEO, Liam Ottley, and CTO, Spencer Porter, on the Implications of OpenAI's Recent Announcements for Your Business.</p>
        </a>
        <a class="platform layered-shadow" href="/{$locale}/blog/our_state_of_the_art_natural_language_to_SQL_innovation">
            <div>
                <h3>Our State-of-the-Art Natural Language to SQL Innovation</h3>
                <LinkArrow/>
            </div>
            <p>Get an inside look into how Helikoid AI is surpassing SOTA performance for Natural Language to SQL. </p>
        </a>
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
