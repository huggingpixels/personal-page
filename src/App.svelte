<script>
  import { Col, Container, Row } from "sveltestrap";

  import Header from "./Header.svelte";
  import Intro from "./Intro.svelte";
  import Resume from "./Resume.svelte";
  import Contact from "./Contact.svelte";
</script>

<svelte:head>
  <link
    href="https://fonts.googleapis.com/css?family=Gochi+Hand&display=swap"
    rel="stylesheet" />
</svelte:head>

<Header />
<Intro />
<Resume />
<Contact />
