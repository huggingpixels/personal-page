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

  .right {
    border-left: 2px solid lightgray;
    position: relative;
    overflow: hidden;

    font-family: "Gochi Hand", cursive;
    font-size: 20px;
  }

  .address {
    border-bottom: 3px solid red;
    width: 80%;
    position: absolute;
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

  #stamp {
    width: 80px;
    height: 100px;
    background-color: red;
    float: right;
    transform: rotate(2deg);
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

  #message {
    font-size: 24px;
  }

  #autogram {
    font-family: "Gochi Hand", cursive;
    float: right;
  }
</style>

<div class="content">
  <div class="card">
    <div class="row">
      <div class="column left">
        <p id="message">What doesn't kill you, makes you smaller.</p>
        <p id="autogram">– Mario</p>
      </div>
      <div class="column right">
        <div id="stamp" />
        <p class="address" id="name">Eszter Szücs-Mátyás</p>
        <p class="address" id="email">eszter.szucs.matyas @gmail.com</p>
        <p class="address" id="insta">@huggingpixels</p>
      </div>
    </div>
  </div>
</div>
