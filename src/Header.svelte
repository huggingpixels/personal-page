<script>
  import Cloud from "./Cloud.svelte";
</script>

<style>
  #backdrop {
    height: 20em;
    background-color: aqua;
    overflow: hidden;
  }

  #backdrop:nth-child(2n) {
    animation-delay: 30s;
  }

  #backdrop:nth-child(3n) {
    animation-delay: 10s;
  }
</style>

<div id="backdrop">
  <Cloud />
  <Cloud />
  <Cloud />
  <Cloud />
  <Cloud />
  <Cloud />
</div>
