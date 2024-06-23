<script>
    const features = [
        {
            title: "Custom Chatbot Development",
            text: "We develop custom AI chatbots that act as intelligent assistants, ensuring 24/7 support and rapid query resolution. Our chatbots maximize engagement and productivity, guiding your employees and customers to the information they need and enabling your team to focus on core business imperatives. Partner with us to unlock the power of AI-powered conversations."
        },
        {
            title: "Workflow Automation",
            text: "Through our deep understanding of AI and its potential, we design agents that can predictively automate tasks, reducing manual intervention and the chances for human error. Whether you're looking to streamline administrative processes, enhance data operations, or elevate customer interactions, our bespoke autonomous agents are built to integrate seamlessly into your environment."
        },
        {
            title: "Natural Language to SQL",
            text: "Our solution transforms natural language queries into precise SQL statements, allowing users to retrieve, manipulate, and analyze data without the need to understand intricate SQL syntax. Empowering both non-tech professionals and experienced developers alike, we bridge the gap between human language and database queries, making data-driven decisions accessible to all."
        },
        {
            title: "Complex Data Pipelines",
            text: "Our expertise lies in designing and deploying data pipelines that handle large-scale, multi-dimensional data. Whether you're dealing with real-time data streams, batch processing, or a hybrid, our autonomous agents optimize processes, ensuring data integrity, and timely delivery for advanced analytics and machine learning applications."
        },
        {
            title: "Self-Adaptive Decision Systems",
            text: "Our self-adaptive solutions harness the full potential of autonomous agents, enabling them to make decisions based on real-time data, past experiences, and predictive analytics. This continuous loop of learning and adapting ensures that your business stays ahead of the curve, optimizing operations and strategizing for future scenarios."
        },
        {
            title: "Use Case Identification",
            text: "Our consultants engage in a deep-dive analysis of your organization's operations, culture, and aspirations. By weaving together this understanding with our vast knowledge of AI advancements, we illuminate AI opportunities that resonate with your business objectives and industry dynamics."
        }
    ]
</script>
<div class="wrapper">
    <h2>Our Services</h2>
    <p>Our news and media information</p>
</div>
<div class="features">
    {#each features as card}
        <div class="layered-shadow">
            <h2>{card.title}</h2>
            <p>{card.text}</p>
        </div>
    {/each}
</div>

<style lang="scss">
  .wrapper {
    h2 {
      font-size: 3rem;

      @media screen and (max-width: 568px) {
        font-size: 2rem;
      }
    }
    p {
      margin: 0;
    }
  }
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
