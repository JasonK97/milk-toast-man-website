<template>
  <div id="footer">
    <a width="854" height="480" href="https://www.youtube.com/channel/UCVDFQ1SkdAHL4pYbnHGYkaA" target="_blank"><img src="@/assets/youtubelogo.png"
        alt="Youtube Icon" height="30"></a><br /><br />
    <a id="footerText" href="mailto:mtm_music@outlook.com">mtm_music@outlook.com</a>
    <p id="footerText">&copy;{{ year }} milk toast man</p>
  </div>
</template>

<script>
export default {
  data () {
    return {
      year: new Date().getFullYear()
    }
  }
}
</script>
