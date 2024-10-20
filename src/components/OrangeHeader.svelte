<script lang="ts">
  import ArrowImg from "../assets/images/icon-arrow-down.svg";
  import LogoImg from "../assets/images/logo.svg";

  export let title:string;
</script>

<header class="header">
  <nav class="header-nav">
    <img class="header-logo" src={LogoImg} alt="logo" />
    <ul class="header-nav-ul">
      <li>
        <a href="#"> About</a>
      </li>
      <li>
        <a href="#">Services</a>
      </li>
      <li>
        <a href="#">Projects</a>
      </li>
      <li>
        <button type="button" class="header-btn"> CONTACT </button>
      </li>
      <li></li>
    </ul>
  </nav>
  <h1>{title}</h1>
  <a href="#bottom">
    <img class="header-arrow" src={ArrowImg} alt="Arrow" />
  </a>
</header>
