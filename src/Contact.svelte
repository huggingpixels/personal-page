<style>
  #insta {
    text-decoration: none;
    color: var(--darkyellow);
    font-family: var(--Handwriting);
    line-height: 1em;
    font-size: var(--Medium);
        background-color: var(--darkgray);
    padding: var(--Small);
    border-radius: var(--Small);
    left: 95px;
    top: 20px;
    position: relative;
  }

  .content {
    width: 50vw;
    position: relative;
    top: 130px;
    left: -195px;
    transform: rotate(-7deg);
  }

  .card {
    display: flex;
    flex-grow: 1;
    flex-basis: 0;

    height: 400px;
    max-width: 800px;
    min-width: 600px;
    background-color: var(--white);

    border: 10px solid red;
    border-image: repeating-linear-gradient(
        45deg,
        var(--lightrose),
        var(--lightrose) 2%,
        var(--darkblue) 1%,
        var(--darkblue) 4%
      )
      10;
  }

  .right {
    border-left: 2px dashed var(--darkgray);
    position: relative;
    overflow: hidden;
    font-size: var(--Small);
    color: var(--darkblue);
  }

  .address {
    border-bottom: 3px solid var(--lightrose);
    width: 90%;
    position: absolute;
    font-family: var(--Oswald);
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
    background-color: var(--lightblue);
    border: 5px dotted var(--white);
    float: right;
    transform: rotate(2deg);
  }

  #name {
    bottom: 100px;
  }

  #email {
    bottom: 10px;
  }
</style>

<div>
  <a href="https://www.instagram.com/huggingpixels/" id="insta">
    @huggingpixels
  </a>
</div>

<div class="content">
  <div class="card">
    <div class="row">
      <div class="column left" />
      <div class="column right">
        <div id="stamp" />
        <p class="address" id="name">Eszter Szücs-Mátyás</p>
        <p class="address" id="email">eszter.szucs.matyas @gmail.com</p>
      </div>
    </div>
  </div>
</div>
