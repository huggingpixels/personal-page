<script>
  import { Card, Col, Row } from "sveltestrap";
</script>

<style>
  .content {
    padding: 0 50px 0 50px;
    justify-content: center;
  }

  .card {
    display: flex;
    flex-grow: 1;
    flex-basis: 0;

    height: 400px;
    max-width: 600px;
    background: white;
    color: black;

    border: 10px solid red;
    border-image: repeating-linear-gradient(
        45deg,
        red,
        red 2%,
        blue 1%,
        blue 4%
      )
      10;
    box-shadow: 0 3px 6px rgba(0, 0, 0, 0.16), 0 3px 6px rgba(0, 0, 0, 0.23);
  }

  .left {
    border-right: 1px solid black;
    position: relative;
    overflow: hidden;

    font-family: "Liu Jian Mao Cao", cursive;
    font-size: 26px;
  }

  p {
    border-bottom: 3px solid red;
    width: 80%;
    position: absolute;
  }

  #name {
    bottom: 150px;
  }

  #insta {
    bottom: 100px;
  }

  #email {
    bottom: 50px;
  }

  .row {
    display: flex;
    width: 100%;
  }

  .column {
    flex: 50%;
    flex-basis: 0;
    padding: 10px;
  }
</style>

<div class="content">
  <div class="card">
    <div class="row">
      <div class="column left">
        <p id="name">firstname lastname</p>
        <p id="email">eszter.szucs.matyas @gmail.com</p>
        <p id="insta">@huggingpixels</p>
      </div>
      <div class="column right">Goodbye Cruel World</div>
    </div>
  </div>
</div>
