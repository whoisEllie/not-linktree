<script>
    import Listitem from "$lib/components/listitem.svelte";


</script>

<div class="wrapper">
  <div class="grid">
    <div class="namecard">
        <img src="pfp.jpg" alt="Ellie smiling at the camera" class="pfp"/>
      <div>
        <div style="font-size: 24px;">
          Ellie Kelemen
        </div>
        <div>
          Software Engineer, Technical Director, Maker
        </div>
      </div>
    </div>
    <div class="links-wrapper">
      <Listitem link="https://www.linkedin.com/in/ellie-kelemen" text="LinkedIn" iconslug="linkedin"/>
      <div class="spacer"></div>
      <Listitem link="https://www.github.com/whoisellie" text="Github" iconslug="github"/>
      <div class="spacer"></div>
      <Listitem link="https://www.youtube.com/@elliemakesgames" text="YouTube" iconslug="youtube"/>
    </div>
    <div on:click={() => window.open("https://github.com/whoisEllie/not-linktree")} class="acknowledgment">
        {"Built with ❤️  & SvelteKit"}
    </div>
  </div>
</div>

<style>

:global(body) {
  margin: 0;
  padding: 0;
}

.wrapper {
  height: 100svh;
  width: 100vw;
  display: flex;
  justify-content: center;
  background: #f0f0f0;
  align-items: center;
}

.grid {
  display: grid;
  grid-template-rows: auto auto auto;
}

.namecard {
  display: grid;
  grid-template-columns: repeat(2, 50%);
  column-gap: 1rem;
  justify-content: center;
  font-family: "tajawalmedium";
  align-items: center;
  padding: 2.5rem 1.5rem;
}

.pfp {
  display: flex;
  aspect-ratio: 1/1;
  background: red;
  width: 100%;
  height: 100%;
  border-radius: 100%;
  object-fit: cover;
}

.links-wrapper {
  display: flex;
  flex-direction: column;
  width: min(100vw - 2rem, 440px);
  margin-inline: auto;
  background: rgb(131,58,180);
  background: linear-gradient(135deg, rgba(131,58,180,1) 0%, rgba(253,29,29,1) 50%, rgba(252,176,69,1) 100%);
  border-radius: 25px;
  background: linear-gradient(145deg, #d8d8d8, #ffffff);
  box-shadow:  20px 20px 39px #cacaca,
               -20px -20px 39px #ffffff;
}

.spacer {
  height: 2pt;
  background: #00000010;
}

.acknowledgment {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0.5rem 1rem;
  width: max-content;
  margin: 2rem auto;
  cursor: pointer;
  font-family: "tajawalmedium";
  border-radius: 25px;
  background: linear-gradient(145deg, #d8d8d8, #ffffff);
  box-shadow:  9px 9px 17px #cacaca,
             -9px -9px 17px #ffffff;

}


</style>
