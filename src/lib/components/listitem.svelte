<script>

  export let link;
  export let text;
  export let iconslug;

</script>

<button on:click={() => window.open(link)} class="link-panel">
  <img height="24" width="24" src="https://cdn.jsdelivr.net/npm/simple-icons@v13/icons/{iconslug}.svg" />
  {text}
</button>

<style>

.link-panel {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 2rem 0;
  color: black;
  text-decoration: none;
  font-size: 1.75rem;
  font-family: "tajawalbold";
  border: none;
  background: transparent;
  cursor: pointer;
}

.link-panel img {
  padding: 0 0.5rem 0 0;
}

</style>
