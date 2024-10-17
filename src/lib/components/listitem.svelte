<script>

  export let link;
  export let text;

</script>

<button on:click={() => window.open(link)} class="link-panel">
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

</style>
