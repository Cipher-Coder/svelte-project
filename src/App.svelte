<script>
  import Header from "./components/Header.svelte";
  import Card from "./components/Card.svelte";

  let intro = "Let's practice some skills!!!";

  const pkg = {
    title: "Math Facts!",
    src: "../assets/img/kidBlackboard.jpg",
    altText: "Cartoon of child in front of blackboard",
    aHref: "#",
    desc: "Practice Your Math!"
  };

  const art = {
    title: "Vocabulary",
    src: "../assets/img/boyReading.jpg",
    altText: "Cartoon of child reading book",
    aHref: "#",
    desc: "Practice Your Spelling!"
  };
</script>

<style>
  h1 {
    color: #000000;
    text-align: center;
  }
</style>

<Header />

<h1>{intro}!</h1>
<div class="menu-container">
  <Card {...pkg} />
  <Card {...art} />
</div>
