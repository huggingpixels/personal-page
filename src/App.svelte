<script>
  import Header from "./Header.svelte";
  import Intro from "./Intro.svelte";
  import Resume from "./Resume.svelte";
  import Contact from "./Contact.svelte";
</script>

<svelte:head>
  <link
    href="https://fonts.googleapis.com/css2?family=Abril+Fatface&family=Oswald:wght@500&family=Roboto&family=Rock+Salt&display=swap"
    rel="stylesheet" />
</svelte:head>

<style>
div {
  display: table;
  margin: var(--Small) 0 var(--Small) 0;
  height:auto;
  width: auto;
}
</style>

<div>
  <Header />
  <Intro />
  <Resume />
  <Contact />
</div>
