<script lang="ts">
  import type { Content } from "../Data.ts";
  import FirstImg from "../assets/images/image-emily.jpg";
  import SecondImg from "../assets/images/image-thomas.jpg";
  import ThirdImg from "../assets/images/image-jennie.jpg";

  interface Props {
    subTitle: string;
  }

  let { subTitle }: Props = $props();

  const testimonialsData: Content = {
    cellBlocks: [
      {
        heading: `Marketing Director`,
        title: `Emily R.`,
        content: `We put our trust in Sunnyside and they 
      delivered, making sure our needs were met 
      and deadlines were always hit`,
      },
      {
        heading: `Chief Operating Officer`,
        title: `Thomas S.`,
        content: `
      Sunnyssides enthusiam coupled with their 
      keen interest in our brand's success made it a satisfying
      and enjoyable experience.
      `,
      },
      {
        heading: `Business Owner`,
        title: `Jennie F.`,
        content: `
      Incredible end result! Our sales increased
      over 400% when we worked with Sunnyside. 
      Highly recommended!
      `,
      },
    ],
  };
</script>

<h3 class="testimonials-heading center">{subTitle}</h3>
<div class="testimonials-container">
  <div class="testimonials-inner-container">
    <img class="testimonials-img" src={FirstImg} alt="emily" />
    <div class="testimonials-mt">
      <p class="testimonials-padding">
        {testimonialsData.cellBlocks[0].content}
      </p>
      <div class="testimonials-mt">
        <span class="testimonials-names">
          {testimonialsData.cellBlocks[0].title}
        </span>
        <p class="testimonials-positions">
          {testimonialsData.cellBlocks[0].heading}
        </p>
      </div>
    </div>
  </div>
  <div class="testimonials-inner-container">
    <img class="testimonials-img" src={SecondImg} alt="thomas" />
    <div class="testimonials-mt">
      <p class="testimonials-padding">
        {testimonialsData.cellBlocks[1].content}
      </p>
      <div class="testimonials-mt">
        <span class="testimonials-names">
          {" "}
          {testimonialsData.cellBlocks[1].title}
        </span>
        <p class="testimonials-positions">
          {" "}
          {testimonialsData.cellBlocks[1].heading}
        </p>
      </div>
    </div>
  </div>
  <div class="testimonials-inner-container">
    <img class="testimonials-img" src={ThirdImg} alt="jennie" />
    <div class="testimonials-mt">
      <p class="testimonials-padding">
        {testimonialsData.cellBlocks[2].content}
      </p>
      <div class="testimonials-mt">
        <span class="testimonials-names">
          {testimonialsData.cellBlocks[2].title}
        </span>
        <p class="testimonials-positions">
          {testimonialsData.cellBlocks[2].heading}
        </p>
      </div>
    </div>
  </div>
</div>
