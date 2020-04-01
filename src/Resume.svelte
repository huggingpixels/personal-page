<script>
  function takeToCV() {
    window.open("https://www.linkedin.com/in/eszter-szucsmatyas/");
  }
</script>

<style>
  @media all and (min-width: 600px) {
    .container {
      display: flex;
      margin: var(--Small);
      float: right;
    }
    .right-container {
      max-width: 50vw;
    }
  }

  @media all and (max-width: 599px) and (min-width: 320px) {
    .container {
      display: block;
      margin: var(--Small);
    }
    .right-container {
      width: 90vw;
    }
  }

  .right-container {
    color: var(--white);
    font-family: var(--Oswald);
    font-size: var(--Medium);
    background-color: var(--lightrose);
    padding: var(--Small);
    border-radius: var(--Small);
  }

  button {
    cursor: pointer;
    width: 180px;
    height: 180px;
    border-radius: 50%;
    background-image: linear-gradient(
      to bottom right,
      var(--lightyellow) 10%,
      var(--darkyellow) 30%
    );

    display: flex;
    align-items: center;
    justify-content: center;

    margin: 5vw;
  }

  .coin-center {
    width: 125px;
    height: 125px;
    border-radius: 50%;
    background-image: linear-gradient(
      to bottom right,
      var(--lightyellow) 20%,
      var(--darkyellow) 70%,
      var(--lightyellow) 100%
    );
    border: 0.2px solid var(--shadowyellow);
    box-shadow: -4px -4px var(--shadowyellow);

    display: flex;
    align-items: center;
    justify-content: center;
  }

  em {
    font-weight: 800;
    font-size: 10vh;
    font-style: normal;
    color: var(--darkyellow);
    text-shadow: 3px 2px 3px var(--shadowyellow);
  }
</style>

<div class="container">
  <div class="left-container">
    <button on:click={takeToCV}>
      <p class="coin-center">
        <em>$</em>
      </p>
    </button>
  </div>
  <div class="right-container">
    <span>
      My LinkedIn page is a great place to get to know my resume, click on the
      coin on the left to travel there.
    </span>
  </div>
</div>
