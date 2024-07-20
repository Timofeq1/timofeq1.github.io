<script>
	import BackgroundVideo from './components/background1.svelte';
</script>

<main>
  <BackgroundVideo />
  <div class="content">
    <h1>Welcome to My Site</h1>
    <p>This is the content over the video background.</p>
  </div>
</main>

<style>
  main {
    position: relative;
    overflow: hidden;
  }

  .content {
    position: relative;
    z-index: 1;
    color: white;
    text-align: center;
    padding-top: 20%;
  }
</style>