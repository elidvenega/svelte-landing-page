<script lang="ts">
  let isOpen = false;

  const handleToggleMenu = () => {
    isOpen = !isOpen;
  };
</script>

<div class="hamburger-menu">
  <!-- svelte-ignore a11y-click-events-have-key-events -->
  <!-- svelte-ignore a11y-no-static-element-interactions -->
  <div class="hamburger-icon" on:click={handleToggleMenu}>
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
  </div>
  <nav class={`hamburger-nav ${isOpen ? "open" : ""}`}>
    <ul class={`menu-items ${isOpen ? "open" : ""}`}>
      <!-- svelte-ignore a11y-invalid-attribute -->
      <li><a href="#">About</a></li>
      <!-- svelte-ignore a11y-invalid-attribute -->
      <li><a href="#">Services</a></li>
      <!-- svelte-ignore a11y-invalid-attribute -->
      <li><a href="#">Projects</a></li>
      <li>
        <button class="menu-items-button" type="button">Contact</button>
      </li>
    </ul>
  </nav>
</div>
