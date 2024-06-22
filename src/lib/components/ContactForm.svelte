<script>
import {fade} from "svelte/transition";

</script>

<div class="app">
    <div class="wrapper">
        <div class="col left">
            <div class="nav">
                <h1>Hugin</h1>
                <p>This is a live feed from our decentralized encrypted privacy messenger. </p>
            </div>
            <div class="action small">
                <h2>Want to join the conversation?</h2>
                <p>Download Hugin Messenger and get 5 XKR to start chatting straight away!</p>
            </div>
        </div>
    </div>
</div>

<style lang="scss">

  .app {
    width: 100%;
    overflow: hidden;
  }

    .wrapper {
      display: flex;
      height: 100vh;

      @media only screen and (max-width: 700px) {
        flex-direction: column;
      }

      .action-mobile {
        display: none;

        p {
          margin-bottom: 2rem;
        }


        @media only screen and (max-width: 700px) {
          display: block;
        }

      }
    }

    .action {
      p {
        margin-bottom: 2rem;
      }
    }

    .posts {
      display: flex;
      padding: 2rem;
      flex-direction: column;
      gap: 10px;
      width: 100%;
      overflow: scroll;
      -ms-overflow-style: none;
      scrollbar-width: none;
      border-right: 1px solid var(--border-color);
      border-left: 1px solid var(--border-color);

      @media only screen and (max-width: 1000px) {
        padding: 2rem 0 2rem 2rem;
        border-right: none;
      }

      @media only screen and (max-width: 700px) {
        margin-top: 40px;
        padding: 0;
        border-left: none;
      }

      &::-webkit-scrollbar {
        display: none;
      }
    }

    .post {
      background-color: var(--card-background);
      border: 1px solid var(--card-border);
      padding: 1rem;
      border-radius: 0.4rem;
      -ms-word-break: break-word;
      word-break: break-word;

      -webkit-hyphens: auto;
      -moz-hyphens: auto;
      hyphens: auto;

      h4 {
        margin: 0;
        white-space: nowrap;
        max-width: 100px;
        overflow: hidden;
        text-overflow: ellipsis
      }
      h5 {
        margin: 0;
      }

      p {
        margin: 10px 0 0 0;
      }
    }

    .col {
      box-sizing: border-box;
      display: flex;
      flex-direction: column;
      max-width: 250px;
      width: 100%;
    }

    .right {
      padding-left: 2rem;

      @media only screen and (max-width: 1000px) {
        display: none;
      }
    }

    .left {
      display: flex;
      flex-direction: column;
      padding-bottom: 2rem;
      padding-right: 2rem;

      p {
        margin: 0;
      }

      @media only screen and (max-width: 700px) {
        display: none;
      }

      .small {
        display: none;

        @media only screen and (max-width: 1000px) {
          display: block;
        }
      }
    }

  .nav {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
    .nav-link {
      box-sizing: border-box;
      display: flex;
      align-items: center;

      h3 {
        margin: 0;
      }
    }

</style>
