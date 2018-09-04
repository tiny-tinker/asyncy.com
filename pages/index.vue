<template>
  <div>
    <section class="intro-section">
      <div class="container">
        <h2 class="display-1 text-center">Build smarter applications</h2>
        <h3 class="text-muted text-center mb-5">
          Supercharge developers to build and scale applications lightning fast ⚡
        </h3>

        <form class="row mb-5">
          <div class="col-12 col-lg-8 offset-lg-2 d-flex">
            <div class="flex-grow-1 pl-3 pr-3">
              <a-input placeholder="Enter Email" inputClasses="bg-light border-none text-dark" />
            </div>
            <div>
              <a-button type="default">Join Beta</a-button>
            </div>
          </div>
        </form>

        <a-player class="intro-video">
          <div class="plyr__video-embed">
          <iframe
              src="https://player.vimeo.com/video/89527215?loop=false&amp;byline=false&amp;portrait=false&amp;title=false&amp;speed=true&amp;transparent=0&amp;gesture=media"
              allowfullscreen allowtransparency allow="autoplay">
            </iframe>
          </div>
        </a-player>
      </div>
    </section>

    <section class="examples-section">
      <div class="container">
        <h3 class="text-center mb-5">
          <a-wordmark/> is a <strong>DLS</strong> powered <strong>platform</strong> that manages <strong>serverless microservices</strong>
        </h3>
        <a-tabs center bold tabShape="links" class="flex-column flex-md-row">
          <div>
            <a-tab-pane title="Serverless HTTP">
              <div class="serverless-tabpane">
                <div class="left-part">
                  <div class="row">
                    <div class="col-12">
                      <img class="w-100" src="@/assets/img/repl.png" role="presentation" alt="asyncy examples">
                    </div>
                  </div>
                  <div class="row mt-3">
                    <div class="col-6">
                      <img class="w-100" src="@/assets/img/logs.png" role="presentation" alt="asyncy examples">
                    </div>
                    <div class="col-6">
                      <img class="w-100" src="@/assets/img/metrics.png" role="presentation" alt="asyncy examples">
                    </div>
                  </div>
                </div>
                <div class="right-part">
                  <img class="w-100" src="@/assets/img/slack.png"/>
                </div>
              </div>
            </a-tab-pane>

            <a-tab-pane title="Slack Bot">
              <p class="description">Cosby sweater eu banh mi, qui irure terry richardson ex squid. Aliquip placeat salvia cillum iphone. Seitan aliquip quis cardigan american apparel, butcher voluptate nisi qui.</p>
            </a-tab-pane>

            <a-tab-pane title="Machine Learning">
              <p class="description">Raw denim you probably haven't heard of them jean shorts Austin. Nesciunt tofu stumptown aliqua, retro synth master cleanse. Mustache cliche tempor, williamsburg carles vegan helvetica. Reprehenderit butcher retro keffiyeh dreamcatcher synth.</p>
            </a-tab-pane>
          </div>
        </a-tabs>
      </div>
    </section>

    <section class="developer-first-tooling">
      <h2 class="display-1 text-center">Developer-First Tooling</h2>
      <a-tabs center bold tabNavLinkClasses="color-gray" tabShape="icon-only" class="flex-column flex-md-row">
        <div>
          <a-tab-pane>
            <template slot="title">
              <div class="h4">
                <i class="fa fa-windows mr-2"></i>
              </div>
            </template>
            <a-snippet center size="lg" prependText=">" value="brew install asyncy/brew/asyncy"></a-snippet>
          </a-tab-pane>

          <a-tab-pane title="Slack Bot">
              <template slot="title">
                  <div class="h4">
                      <i class="fa fa-apple mr-2"></i>
                  </div>
              </template>
              <a-snippet center size="lg" prependText="$" value="brew install asyncy/brew/asyncy"></a-snippet>
          </a-tab-pane>

          <a-tab-pane title="Machine Learning">
              <template slot="title">
                  <div class="h4">
                      <i class="fa fa-linux mr-2"></i>
                  </div>
              </template>
              <a-snippet center size="lg" prependText="$" value="brew install asyncy/brew/asyncy"></a-snippet>
          </a-tab-pane>
        </div>
      </a-tabs>
      <h4 class="display-4 text-center mt-5 mb-4">Install the Asyncy CLI to get started</h4>
      <a-button type="primary" outline>Read the Documentation</a-button>
    </section>

    <section class="cards-section">
      <div class="container">
        <div class="row cards">

          <div class="col-md-12 col-lg-4" v-for="card in cards" :key="card.id">
            <a-card shadow class="h-100" bodyClasses="cards-card-body">
              <template slot="header">
                <div class="image-container">
                  <img v-if="card.leftImg" :src="card.leftImg" :alt="card.title" class="storyscript-left">
                  <img v-if="card.img" :src="card.img" :alt="card.title" class="w-100">
                  <img v-if="card.rightImg" :src="card.rightImg" :alt="card.title" class="storyscript-right">
                </div>
              </template>

              <h4 class="display-4">{{ card.title }}</h4>
              <p> {{ card.description }}</p>
              <a href="#" class="btn btn-link text-primary">Learn more</a>
            </a-card>
          </div>

        </div>
      </div>
    </section>

    <section class="benefit-section">
      <div class="container">
        <div class="row">
          <div class="col-sm-12 col-lg-6" v-for="benefit in benefits" :key = "benefit.id" >
            <a-card class="flex-row">
              <template slot="header">
                <img src="@/assets/img/benefit-placeholder.svg" alt="asyncy benefit">
              </template>
              <h4 class="display-4">{{benefit.title}}</h4>
              <p>{{benefit.description}}</p>
            </a-card>
          </div>
        </div>

        <h4 class="text-center mt-5 mb-5">Have questions? Read our <span class="text-primary">FAQ</span> to learn more</h4>
      </div>
    </section>

    <section class="open-source-section">
      <img src="@/assets/img/nebula.png">
      <div class="container">
        <div class="content">
          <h3 class="color-white mb-4">WE ARE <strong>OPEN</strong> SOURCE</h3>
          <h4 class="display-4 color-white text-center">Platfrom   •   Language   •   Standards   •   Cloud</h4>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
  import storyscript from '@/assets/img/storyscript.png';
  import storyscriptLeft from '@/assets/img/storyscript-left.png';
  import storyscriptRight from '@/assets/img/storyscript-right.png';
  import dashboard from '@/assets/img/dashboard.png';
  import hub from '@/assets/img/hub.png';

  export default {
    data() {
      return {
        benefits: [
          {
            id: '1',
            title: 'Horizontal scaling from  0 → ∞ → 0',
            description: 'No cold-restarts, your services are always hot-and-ready but scale to 0 to reduce costs and scale to N.',
          },
          {
            id: '2',
            title: 'Zero to Hero',
            description: 'Rapidly prototype applications in a production -grade platform.'
          },
          {
            id: '3',
            title: 'Micro scaling',
            description: 'Services scale independently and automatically to reduce bottlenecks and improve throughput.'
          },
          {
            id: '4',
            title: 'Smarter libraries',
            description: 'Discover and build services built on open standards that are smarter than your average library.'
          },
          {
            id: '5',
            title: 'AB testing',
            description: 'Built-in AB testing of Stories and services to ensure your application performs flawlessly.'
          },
          {
            id: '6',
            title: 'Goal-oriented programming',
            description: 'Remove unnecessary complexity from application goals and you are left transparent business logic.'
          }
        ],
        cards: [
          {
            id: '1',
            img: storyscript,
            leftImg: storyscriptLeft,
            rightImg: storyscriptRight,
            title: 'StoryScript',
            description: 'Goal-oriented Cloud Native Programming Language that defines how data flows through applications in trasparent and intuitive syntax.'
          },
          {
            id: '2',
            img: dashboard,
            title: 'Dashboard',
            description: 'Application insight, metrics and management for teams to grow and scale products from day one.'
          },
          {
            id: '3',
            img: hub,
            title: 'Hub',
            description: 'Choose from hundreds of community supported services and build your own in any programming lanugage.'
          }
        ]
      }
    }
  }
</script>

<style lang="scss">
  .intro-section {
    .intro-video {
      margin: 50px 0 75px 0;
    }
  }

  .examples-section {
    .serverless-tabpane {
      display: flex;
      flex-direction: row;

      .left-part {
        flex-grow: 7;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
      }
      .right-part {
        flex-grow: 6;
        padding-left: 2rem;
      }
      @media screen and (max-width: 767px) {
        flex-direction: column;

        .right-part {
          margin-top: 3rem;
          padding-left: 0;
        }
      }
    }
  }

  .developer-first-tooling{
    padding: 150px 0;
    display: flex;
    align-items: center;
    flex-flow: column;
  }

  .cards-section {
    padding: 90px 0;
    overflow: hidden;

    .cards {
      margin-top: 50px;

      > div {
        @media screen and (max-width: 991px) {
          margin-top: 180px;

          &:first-child {
            margin-top: 0;
          }
        }
      }

      .card {
        border-radius: 1.25rem;
        max-width: 350px;
        margin: 0 auto;
      }

      .cards-card-body {
        display: flex;
        flex-flow: column;
        justify-content: space-between;
        align-items: flex-start;
        height: 100%;
      }

      .card-header {
        border-bottom: none;
        background: white;
        border-radius: 1.25rem;

        .image-container {
          position: relative;
          margin-top: -50%;
          width: 95%;
          left: 2.5%;

          .storyscript-left, .storyscript-right {
            position: absolute;
            height: 100%;
          }

          .storyscript-left {
            right: 100%;
            margin-left: -100%;
          }

          .storyscript-right {
            left: 100%;
            margin-right: 100%;
          }
        }
      }
    }
  }

  .benefit-section {
    .card {
      border: none;
    }

    .card-header {
      display: flex;
      background-color: transparent;
      border-bottom: none;
      align-items: center;
      justify-content: center;
      padding: 1.25rem 0.5rem;
      height: 100%;

      @media screen and (max-width: 767px) {
        img {
          width: 70px;
        }
      }
    }
  }

  .open-source-section {
    position: relative;
    overflow: hidden;

    > img {
      width: 100%;

      @media screen and (max-width: 767px) {
        width: unset !important;
        height: 380px;
      }
    }

    .content {
      position: absolute;
      display: flex;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      padding-top: 10%;
      flex-flow: column;
      align-items: center;
      justify-content: center;

      @media screen and (max-width: 767px) {
        padding-top: 30%;
      }

      @media screen and (max-width: 413px) {
        padding-top: 50%;
      }
    }
  }
</style>

