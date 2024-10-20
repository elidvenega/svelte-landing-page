<script lang="ts">
  import Facebook from "../assets/images/icon-facebook.svg";
  import Instagram from "../assets/images/icon-instagram.svg";
  import Twitter from "../assets/images/icon-twitter.svg";
  import Pinterest from "../assets/images/icon-pinterest.svg";
  import type { Content } from "../Data";

  const footerLinks: Content = {
    cellBlocks: [
      {
        link: {
          href: "https://www.facebook.com/",
        },
      },
      {
        link: {
          href: "https://www.instagram.com/",
        },
      },
      {
        link: {
          href: "https://twitter.com/",
        },
      },
      {
        link: {
          href: "https://www.pinterest.com/",
        },
      },
    ],
  };

  const firstHref = footerLinks.cellBlocks[0]?.link?.href;
  const secondHref = footerLinks.cellBlocks[1]?.link?.href;
  const thirdHref = footerLinks.cellBlocks[2]?.link?.href;
  const fourthHref = footerLinks.cellBlocks[3]?.link?.href;
</script>

<footer class="footer" id="bottom">
  <h4>sunnyside</h4>
  <div class="footer-nav">
    <nav>
      <ul>
        <li>
          <a href="#">About</a>
        </li>
        <li>
          <a href="#">Services</a>
        </li>
        <li>
          <a href="#">Projects</a>
        </li>
      </ul>
    </nav>
  </div>
  <div class="footer-image-links">
    <a href={firstHref} target="_blank">
      <img src={Facebook} alt="facebook" />
    </a>
    <a href={secondHref} target="_blank">
      <img src={Instagram} alt="instagram" />
    </a>
    <a href={thirdHref} target="_blank">
      <img src={Twitter} alt="twitter" />
    </a>
    <a href={fourthHref} target="_blank">
      <img src={Pinterest} alt="pinterest" />
    </a>
  </div>
</footer>
