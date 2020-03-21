<script>
  import { Col } from "sveltestrap";
  import Cloud from "./Cloud.svelte";
</script>

<style>
  #backdrop {
    height: 20em;
    width: 100%;
    overflow: hidden;
  }

  #backdrop:nth-child(2n) {
    animation-delay: 30s;
  }

  #backdrop:nth-child(3n) {
    animation-delay: 10s;
  }

  h1 {
    color: coral;
    font-size: 10em;
  }
</style>

<div id="backdrop">
  <Col>
    <h1>Hello!</h1>
    <Cloud />
    <Cloud />
    <Cloud />
  </Col>
</div>
