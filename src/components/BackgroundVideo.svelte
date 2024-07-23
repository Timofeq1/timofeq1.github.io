<!-- src/components/BackgroundVideo.svelte -->
<style>
  .video-background {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -1; /* Ensure the video stays in the background */
  }
</style>

<video class="video-background" autoplay muted loop>
  <source src="public\background1.mp4" type="video/mp4" />
</video>
