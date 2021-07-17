<template>
  <div class="musicPlayer" :class="{'open':showPlayer}">
    <div class="player">
      <div class="slider" @click="showPlayer = !showPlayer">
        <img src="../assets/music-notes.png" />
      </div>
      <iframe class="bandcamp" src="https://bandcamp.com/EmbeddedPlayer/album=1187034659/size=large/bgcol=ffffff/linkcol=63b2cc/transparent=true/" seamless><a href="https://milktoastman.bandcamp.com/album/brink">Brink by milk toast man</a></iframe>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      showPlayer: false
    }
  }
}
</script>

<style scoped></style>
