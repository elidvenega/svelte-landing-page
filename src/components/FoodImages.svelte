<script lang="ts">
  import MilkImg from "../assets/images/desktop/image-gallery-milkbottles.jpg";
  import OrangePlate from "../assets/images/desktop/image-gallery-orange.jpg";
  import Cone from "../assets/images/desktop/image-gallery-cone.jpg";
  import SugarCubes from "../assets/images/desktop/image-gallery-sugarcubes.jpg";

  const foodImages: string[] = [MilkImg, OrangePlate, Cone, SugarCubes];
</script>

<div class="food-images-container">
  {#each foodImages as foodImage}
    <img class="food-images" src={foodImage} alt="food-images" />
  {/each}
</div>
