<script setup>
import { ref } from "vue";

const glazedOpen = ref(false);
const fritterOpen = ref(false);
const sandwichOpen = ref(false);

function readMore(listing) {
  if (listing == "glazed") {
    glazedOpen.value = !glazedOpen.value;
  } else if (listing == "fritter") {
    fritterOpen.value = !fritterOpen.value;
  } else if (listing == "sandwich") {
    sandwichOpen.value = !sandwichOpen.value;
  }
}
</script>

<template>
  <h1>Menu</h1>
  <div id="menu-grid">
    <div class="menu-item">
      <img src="./images/glazed.png" />
      <hr />
      <h2>Classic Glazed*</h2>
      <span>$1.00</span>
      <br />
      <a href="#" @click="readMore('glazed')">{{
        glazedOpen ? "Hide" : "Read more"
      }}</a>
      <div :class="glazedOpen ? 'open' : 'closed'" @click="readMore('glazed')">
        <h2>Classic Glazed</h2>
        <span>
          Sothy drags her daughters back to the kitchen, insisting that they
          help her glaze the donuts. When they protest, she tells them that
          "He's fine... He's Khmer" (14), as if this simple fact means that he
          must be trustworthy. She begins to build her perception of him based
          off of his ethnicity, in some ways connecting herself to him by
          claiming that he's Khmer, and reasoning that that bond means that they
          can trust him.
        </span>
        <br />
        <br />
        <span>
          A glazed donut is like the the basis from which other donuts build
          upon. Likewise, Sothy (and her daughters) begin to build up from the
          man's Khmer-ness to form their perception of him.
        </span>
        <br />
        <br />
        <span>
          Later, Sothy begins to wrestle with the question of whether or not she
          should really be able to trust the man, despite his ethnicity. She
          recalls the danger that she and the shop may be in due to the
          financial issues that she went through with her ex-husband and her
          distant rich uncle-in-law. In all of these trials, a Khmer man was the
          root issue; if they have screwed her over in the past and may do so in
          the future, how can she trust them now? She continues to question this
          until she must make a decision based on it.
        </span>
      </div>
    </div>
    <div class="menu-item">
      <img src="./images/chocolate_glazed.png" />
      <hr />
      <h2>Chocolate Glazed</h2>
      <span>$1.00</span>
    </div>
    <div class="menu-item">
      <img src="./images/sprinkle.png" />
      <hr />
      <h2>Sprinkled</h2>
      <span>$1.00</span>
    </div>
    <div class="menu-item">
      <img src="./images/chocolate_cake.png" />
      <hr />
      <h2>Chocolate Cake</h2>
      <span>$1.00</span>
    </div>
    <div class="menu-item">
      <img src="./images/apple_fritter.png" />
      <hr />
      <h2>Apple Fritter*</h2>
      <span>$1.50</span>
      <br />
      <a href="#" @click="readMore('fritter')">{{
        fritterOpen ? "Hide" : "Read more"
      }}</a>
      <div
        :class="fritterOpen ? 'open' : 'closed'"
        @click="readMore('fritter')"
      >
        <h2>Apple Fritter</h2>
        <span>
          Throughout this story, it is clear that the man is the catalyst for
          all of the things that happen. In a Cambodian centered story, however,
          he himself does not consider himself to be Khmer. Tevy and Kayley both
          wrestle with their ethnic identity, but the man manages to baffle them
          even further by telling them that his family lived in Cambodia but is
          Chinese by blood, and that's why he is not Khmer. Moreso, his father
          told him that he was Chinese, and he followed that seemingly without
          question. Tevy and Kayley question him to challenge this, asking about
          his culture and his holidays, his family's language and the food that
          he eats. Still, he doesn't budge, instead turning the conversation to
          them and challenging their ethnic identity. It's clear from this that
          he doesn't want to be considered Khmer, even though he does many of
          the things that the girls consider Khmer.
        </span>
        <br />
        <br />
        <span>
          Despite this, he still finds himself in a Khmer donut shop every night
          for a while, purchasing something even though he doesn't like donuts.
          He goes to the shop regularly even though the girls whisper and gossip
          about him every time, and it becomes a question of why he even shows
          up there to begin with, especially if he doesn't claim the same ethnic
          identity as them. There's still a strange sense of solidarity between
          him and the girls, which appears to stem from their shared culture.
        </span>
      </div>
    </div>
    <div class="menu-item">
      <img src="./images/egg_sandwich.png" />
      <hr />
      <h2>Egg Sandwich*</h2>
      <span>$4.50</span>
      <br />
      <a href="#" @click="readMore('sandwich')">{{
        sandwichOpen ? "Hide" : "Read more"
      }}</a>
      <div
        :class="sandwichOpen ? 'open' : 'closed'"
        @click="readMore('sandwich')"
      >
        <h2>Egg Sandwich</h2>
        <span>
          Ultimately, the story cumulates in a moment where all three of the
          women of Chuck's Donuts make an assessment within which person they
          will choose to side or align with: “the man, to whose presence they
          have grown attached, or the bruised woman, whose explosive anger
          towards the man appears warranted" (36).
        </span>
        <br />
        <br />
        <span>
          Sothy, directly or indirectly, ends up choosing the woman. We as the
          readers don't know who actually used the egg sandwich cast iron pan to
          hit the man, but regardless of who made the swing, Sothy was the one
          to bring that pan into the scene. She made a choice in the moment to
          either help the man or woman, and both options would have ended the
          fight. This choice was based purely on her perception of their
          characters, but she didn't have the context which Tevy and Kayley had
          from their dialogue.
        </span>
        <br />
        <br />
        <span>
          Because of this lack of context about either character, it is clear
          that Sothy instinctually draws towards another woman even though she's
          seen the man many times. Her past experience with hurt and fear push
          her to trust in this woman despite not knowing who she is at all. She
          could have not interfered with the situation at all, but because she
          felt so strongly about this decision, she made the move.
        </span>
      </div>
    </div>
  </div>
</template>

<style scoped>
#menu-grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  row-gap: 30px;
}

.menu-item {
  text-align: center;
  padding: 10px;
}

img {
  width: 100%;
}

h1 {
  text-align: center;
}

h2 {
  margin-top: 20px;
}

.open,
.closed {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  padding: 200px;
  z-index: 100;
  background-color: rgba(242, 176, 223, 0.95);
  backdrop-filter: blur(10px);
}

.open {
  display: block;
}

.closed {
  display: none;
}
</style>
