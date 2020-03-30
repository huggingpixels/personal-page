<script>
  import { Card, Col, Row } from "sveltestrap";
</script>

<style>
  a {
    text-decoration: none;
    color: var(--darkgreen);
  }
  
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
    background-color: var(--white);

    border: 10px solid red;
    border-image: repeating-linear-gradient(
        45deg,
        var(--darkrose),
        var(--darkrose) 2%,
        var(--darkblue) 1%,
        var(--darkblue) 4%
      )
      10;
  }

  .right {
    border-left: 1px dashed var(--darkblue);
    position: relative;
    overflow: hidden;

    font-family: "Gochi Hand", cursive;
    font-size: 20px;
  }

  .address {
    border-bottom: 3px solid var(--darkrose);
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
    background-color: var(--lightgray);
    border: 5px dotted var(--white);
    float: right;
    transform: rotate(2deg);
  }

  #name {
    bottom: 150px;
  }

  #insta {
    bottom: 130px;
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
        <a
          href="https://www.instagram.com/huggingpixels/"
          class="address"
          id="insta">
          @huggingpixels
        </a>
      </div>
    </div>
  </div>
</div>
