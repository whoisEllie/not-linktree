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
  padding: 1.75rem 0;
  color: black;
  text-decoration: underline 0.1em rgba(0, 0, 0, 0);
  transition: text-decoration-color 300ms;
  font-size: 1.75rem;
  font-family: "tajawalbold";
  border: none;
  background: transparent;
  cursor: pointer;
}

.link-panel img {
  padding: 0 0.5rem 0 0;
}

.link-panel:hover {
  text-decoration-color: rgba(0, 0, 0, 1);
}

</style>
