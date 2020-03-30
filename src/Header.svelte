<script>
  import { Col } from "sveltestrap";
  import Cloud from "./Cloud.svelte";
</script>

<style>
  #backdrop {
    height: 20em;
    width: 100%;
    overflow: hidden;
    margin: var(--Medium);
  }

  #backdrop:nth-child(2n) {
    animation-delay: 30s;
  }

  #backdrop:nth-child(3n) {
    animation-delay: 10s;
  }

  h1 {
    color: var(--darkyellow);
    font-family: var(--Abril);
    font-size: var(--Big);
  }
</style>

<div id="backdrop">
    <h1>Hello!</h1>
    <Cloud />
    <Cloud />
    <Cloud />
</div>
