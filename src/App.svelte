<script>
  import { Col, Container, Row } from "sveltestrap";

  import Header from "./Header.svelte";
  import Intro from "./Intro.svelte";
  import Resume from "./Resume.svelte";
  import Contact from "./Contact.svelte";

</script>
<svelte:head>
  <link href="https://fonts.googleapis.com/css?family=Gochi+Hand&display=swap" rel="stylesheet">
</svelte:head>
<!-- <svelte:head>
  <link
    rel="stylesheet"
    href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" />
</svelte:head> -->

<Row>
  <Header />
</Row>
<Container>
<!-- <Row>
  <Intro />
</Row>
<Row>
  <Resume />
</Row> -->
  <Contact />
</Container>
