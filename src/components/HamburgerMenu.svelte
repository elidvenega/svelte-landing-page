<script lang="ts">
  //   import { useState } from "react";

  // export default function HamburgerMenu() {
  //   const [isOpen, setIsOpen] = useState(false);

  //   const handleToggleMenu = () => {
  //     setIsOpen(!isOpen);
  //   };
</script>

<div class="hamburger-menu">
  <div class="hamburger-icon" onClick={handleToggleMenu}>
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
  </div>
  <nav class={`hamburger-nav ${isOpen ? "open" : ""}`}>
    <ul class={`menu-items ${isOpen ? "open" : ""}`}>
      <li>
        <a href="#">About</a>
      </li>
      <li>
        <a href="#">Services</a>
      </li>
      <li>
        <a href="#">Projects</a>
      </li>
      <li>
        <button class="menu-items-button" type="button"> contact </button>
      </li>
    </ul>
  </nav>
</div>
