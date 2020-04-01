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
    position: relative;
    float: right;
    left: -35vw;
    top: -5vh;
  }

  .content {
    width: 50vw;
    position: relative;
    top: 2vh;
    left: -25vh;
    transform: rotate(-7deg);
  }

  .card {
    display: flex;
    flex-grow: 1;
    flex-basis: 0;

    height: 50vh;
    background-color: var(--white);

    border: 1vh solid red;
    border-image: repeating-linear-gradient(
        45deg,
        var(--lightrose),
        var(--lightrose) 2%,
        var(--darkblue) 1%,
        var(--darkblue) 4%
      )
      10;
  }
  @media all and (min-width: 960px) {
    .card {
      width: 50vw;
    }
  }

  @media all and (max-width: 959px) and (min-width: 600px) {
    .card {
      width: 80vw;
    }
  }

  @media all and (max-width: 599px) and (min-width: 320px) {
    .card {
      width: 120vw;
    }
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
    width: 45%;
    height: 30%;
    background-color: var(--lightblue);
    border: 5px dotted var(--white);
    float: right;
    transform: rotate(2deg);
  }

  #name {
    bottom: 10vh;
  }

  #email {
    bottom: 1vh;
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
