<template>
  <div class="home">
    <div class="parallaxPic">
        <div class="caption">
            <span class="title"><strong>milk toast man</strong></span><br />
            <span class="sub-title"><strong>Unique Sound from Unique Experiences</strong></span>
        </div>
    </div>

    <div id="quote">
        <img id="quotePic" src="@/assets/Pink Mountain Morning.jpg" alt="Watercolor painting of a pink sunrise over mountains behind water." />
        <div id="quoteText">
          <p><strong>Medicine is a science of uncertainty and an art of probability.</strong><br />
              --Sir William Osler</p>
        </div>
    </div>

    <div id="video">
        <iframe src="https://www.youtube.com/embed/S9IGq5kAuiI?controls=0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data () {
    return {}
  }
}
</script>

<style scoped></style>
