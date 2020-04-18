<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About World Folklore Festival"
      subtitle="Something about the festival and the team behind it"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>The Team</h3>
          <p>
            <strong>
              Mission and Goal
            </strong>
          </p>
          <p>
            We are proud in our mission to promote the values received from our forebearers, to conserve the rich cultural
            tapestry we received from the generations before us.
            Our goal is to present exotic cultures from all over the world, to improve interconnectedness and to create a new place
            for all cultures, ethnicities, religions and creeds where they can share without discrimination their traditions,
            where we can all explore and enjoy the picturesque show of dances, songs, costumes and colorful stories preserved though time.
          </p>

          <h3>Our Team</h3>
          <p>
            Our team is made of both veterans of cultural and tourist manifestations and young people dedicated
            to preserving cultural heritage from all over the world.
            We are professionals in what we do and we offer only the best to our participants!
            Our team includes public officials of Diano Marina and different Italian organizations, wide array of volonteers
            and students of College of Tourism of Belgrade, Serbia.
          </p>
          <quote-card />
          <h3>Organization</h3>
          <p>
            The idea behind this manifestation was starting to emerge in the beginning of the 90ies.
            The founder of this manifestation saw the need for cultural preservation and as already in the bussiness of tourism,
            the idea to connect beautiful and pragmatic emerged.
            Today we are proud to share that our members cover 4 continents, 100 countries and numerous organizations from all over
            the world which are proud to be part of our family.
          </p>
        </div>

        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Cool Stuff We Do
              </p>
              <p class="subtitle">
                Sooo Cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Other Cool Things
              </p>
              <p class="subtitle">
                Just as cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                All the cool
              </p>
              <p class="subtitle">
                that is all
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
        </div>
      </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
