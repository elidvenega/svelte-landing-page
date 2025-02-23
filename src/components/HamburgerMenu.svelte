<script lang="ts">
  let isOpen = $state(false);

  const handleToggleMenu = () => {
    isOpen = !isOpen;
  };
</script>

<div class="hamburger-menu">
  <!-- svelte-ignore a11y_click_events_have_key_events -->
  <!-- svelte-ignore a11y_no_static_element_interactions -->
  <div class="hamburger-icon" onclick={handleToggleMenu}>
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
  </div>
  <nav class={`hamburger-nav ${isOpen ? "open" : ""}`}>
    <ul class={`menu-items ${isOpen ? "open" : ""}`}>
      <!-- svelte-ignore a11y_invalid_attribute -->
      <li><a href="#">About</a></li>
      <!-- svelte-ignore a11y_invalid_attribute -->
      <li><a href="#">Services</a></li>
      <!-- svelte-ignore a11y_invalid_attribute -->
      <li><a href="#">Projects</a></li>
      <li>
        <button class="menu-items-button" type="button">Contact</button>
      </li>
    </ul>
  </nav>
</div>
