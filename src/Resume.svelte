<script>
  function takeToCV() {
    window.open("https://www.linkedin.com/in/eszter-szucsmatyas/");
  }
</script>

<style>
  .wrapper {
    display: flex;
    margin: var(--Small);
    float: right;
  }

  .right-container {
    color: var(--white);
    font-family: var(--Oswald);
    font-size: var(--Medium);
    background-color: var(--lightgreen);
    padding: var(--XSmall);
    max-width: 600px;
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

    margin: 30px;
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
    font-size: 90px;
    font-style: normal;
    color: var(--darkyellow);
    text-shadow: 3px 2px 3px var(--shadowyellow);
  }
</style>

<div class="wrapper">
  <div class="left-container">
    <button on:click={takeToCV}>
      <p class="coin-center">
        <em>$</em>
      </p>
    </button>
  </div>
  <div class="right-container">
    <p>
      My LinkedIn page is a great place to get to know my resume, click on the
      coin on the left to travel there.
    </p>
  </div>
</div>
