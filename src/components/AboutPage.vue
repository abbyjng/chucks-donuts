<script setup></script>

<template>
  <h1>About Us</h1>
  <div id="description">
    <span>
      Chuck's Donuts is one of many 24-hour always-open Cambodian-owned donut
      shops in the LA area. Run by a single mother and her two daughters, we
      take pride in our family history and culture and are passionate about what
      we do here. Why donuts? We're inspired by a Cambodian pastry
    </span>
    <em>nom kong</em>
    <span>, and we follow in the steps of the</span>
    <em>"Donut King,"</em>
    <span> Ted Ngoy</span>
    <a
      href="https://www.kcet.org/shows/lost-la/the-cambodian-american-reign-of-doughnut-shops-began-in-this-la-habra-shop"
      >[1]</a
    >
    <span>. We hope that our passion can be tasted through our handiwork.</span>
    <br /><br />
    <span>
      Chuck's Donuts, when originally opened, was located in what seemed like
      the ideal space - the street was bustling with activity and the nightlife
      was strong, which made the 24 hour business worthwhile. However, due to
      the housing crisis and the city declaring bankruptcy, it's not the same
      anymore, and the quiet atmosphere creates an intense space that allows for
      more deliberate situations to occur. Now, Sothy, the owner, must
      deliberate the reasons for her keeping the restaurant as it is and what it
      means to her as her history and her livelihood.
    </span>

    <div id="more-info">
      <div>
        <h2>Location</h2>
        <a
          href="https://www.google.com/maps/place/Christy's+Donuts/@34.1190727,-118.213927,15z/data=!3m1!4b1!4m5!3m4!1s0x80c2c407a0f514b7:0xf189a09de887c71f!8m2!3d34.1190561!4d-118.1970181"
          >5546 York Blvd,<br />Los Angeles, CA 90042</a
        >
      </div>
      <div>
        <h2>Hours</h2>
        <span>Always open, 24 hours everyday</span>
      </div>
    </div>
  </div>
  <div id="people">
    <h1 id="title">Three Women of Chuck's Donuts</h1>
    <div class="person">
      <h3>Sothy</h3>
      <img src="./images/sothy.png" />
      <span>
        Sothy is the owner of Chuck's Donuts, and she carries many
        responsibilities. She not only runs a 24-hour donut shop in a local
        economic downturn, but is also a single mother and must face the
        consequences of her cheating husband.
      </span>
      <br />
      <span>
        This shop originally stemmed from a loan from the family's ex-father's
        uncle. When Sothy found out that her ex-husband had been stealing her
        money which was intended to pay the loan back, she became increasingly
        more afraid of the power that the uncle may hold. She hasn't told this
        to her daughters, which ultimately causes her to face a dilemma between
        the dangers of keeping the donut shop and their need for it as their
        livelihood. She becomes even more protective of the two girls, telling
        them to watch out for him, despite her contradiction to telling them
        that "He's fine... He's Khmer" (14) when they expressed concern over
        leaving him in the front of the shop alone. Her fear of the uncle causes
        her to distrust in the man at her shop, and that fear still stemming
        from her relationship with her ex-husband, another Cambodian man.
      </span>
      <br />
      <span>
        Despite this unbased assumption and fear, it turns out to be a
        reasonable concern, as the man was far from good. By the end of the
        story, she assists the man's wife in knocking him out with her cast iron
        pan, and she experiences a moment of solidarity between her and the
        woman. Throughout the story, Sothy struggles to understand what her
        ex-husband's actions mean for her ability to trust other men in her
        life, especially Khmer ones that surround her, but in this experience
        with the other woman, her thoughts are finally "free of her daughters'
        father" (40).
      </span>
    </div>
    <div class="person">
      <h3>Tevy</h3>
      <img src="./images/tevy.png" />
      <span>
        Tevy is the elder of the two daughters by four years at the age of 16.
        She's taking a philosophy course in high school and spends much of her
        time at the restaurant doing homework and reading a book.
      </span>
      <br />
      <span>
        Despite constantly telling her sister, Kayley, off for staring at and
        contemplating the man who visits their shop every night, Tevy begins to
        take interest in him as well as the nights pass. This interest remains
        due to her philosophy course, as she begins to consider that she could
        use the man as a subject for an essay which she has to write. Her
        thought process regarding the man remains analytical, and she even
        begins to wonder how she can use his presence in her life to her
        advantage, to advance her path to college.
      </span>
      <br />
      <span>
        When Sothy tells Tevy and Kayley that the man is Khmer, Tevy becomes
        even more invested in the man, and she along with her sister begin to
        formulate an interview for the man. She reflects upon her own experience
        of being Khmer, drawing from her experience with her father. This is
        informed by not only her mom's ability to identify the man as Khmer, but
        also her father's reference to her own Khmer-ness when he was still in
        her life, and her distaste for her father shapes this view as well.
      </span>
    </div>
    <div class="person">
      <h3>Kayley</h3>
      <img src="./images/kayley.png" />
      <span>
        Kayley, the youngest of the three women of Chuck's Donuts, assists with
        the store at the young age of 12. Naturally curious out of both her age
        and personality, she shows interest in the man who comes to the
        restaurant from the very first day he shows up. One of the first
        questions she asks about him is whether or not he's Cambodian, which
        Tevy brushes off; however, when Sothy confirms that for them, her view
        shifts, and she even contemplates how he looks similar to her father.
      </span>
      <br />
      <span>
        This conversation is one of the big catalysts that draws the story
        together. Because all three women have their husband/father on their
        minds, they now see the man as something more, as if the revelation
        means more than a resemblance.
      </span>
      <br />
      <span>
        When Kayley and Tevy ultimately witness the man and his wife fighting,
        the two girls "cannot say whom they feel more aligned with - the man, to
        whose presence they have grown attached, or the bruised woman, whose
        explosive anger towards the man appears warranted" (36). The man's
        constant presence in the shop, as well as his similarity to their dad,
        plays a part in their view of him, despite not even knowing his name and
        having only one stilted conversation with him.
      </span>
    </div>
  </div>
</template>

<style scoped>
#people {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
  margin-top: 50px;
}

#more-info {
  display: flex;
  margin-top: 50px;
  gap: 50px;
}

#title {
  grid-column: 1 / 4;
}

.person {
  display: flex;
  flex-direction: column;
}

img {
  height: 300px;
  object-fit: contain;
  margin-bottom: 20px;
}
</style>
