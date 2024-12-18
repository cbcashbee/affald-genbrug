<script>
import image1 from '@/assets/images/vid-screen/glas.png';
import image2 from '@/assets/images/vid-screen/metal.png';
import image3 from '@/assets/images/vid-screen/mad-drik.png';
import image4 from '@/assets/images/vid-screen/toej.png';
import image5 from '@/assets/images/vid-screen/trae.png';
import image6 from '@/assets/images/vid-screen/gips.png';
import Slideshow from '../components/Slideshow.vue';

export default {
  components: { Slideshow },
  data() {
    return {
      slides: [image1, image2, image3, image4, image5, image6],
    };
  },
};

</script>

<template>
    <h2>Genanvendelse</h2>
    <section id="ga">
        <div class="box">
            <h3>Derfor skal du...</h3>
            <div>
                <Slideshow :slides="slides" />
            </div>
            <p id="derfor"><br>Se hvad der sker med affaledet, når du sortere det, i videoerne herover.</p>
        </div>

        <div class="box">
            <h3>Affald i tal</h3>
            <p>Meget af det der sorteres, bliver rent faktisk genanvendt til nye ressourcer. Det er ikke altid at man som borger ved dette, og man kan miste motivationen til at sortere. 
              Men det nytter altså noget, at sortere.
              <br><br>
              Herunder kan du se statistikker på hvad der sker med affaldet i Middelfart kommune:
              <br><br>
</p>
            <img src="../assets/images/genan-pro.png" alt="">
        </div>
    </section>
    <img id="gul" src="../assets/images/boelge-gul.png" alt="Gul bølge">
</template>

<!--
    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="1618" height="442.64" viewBox="0 0 1618 442.64">
  <defs>
    <clipPath id="clip-path">
      <path id="Path_35" data-name="Path 35" d="M0,328.468H1618v-442.64H0Z" transform="translate(0 114.172)" fill="#f5ba3b"/>
    </clipPath>
  </defs>
  <g id="Group_3" data-name="Group 3" transform="translate(0 110.172)">
    <g id="Group_2" data-name="Group 2" transform="translate(0 -110.172)" clip-path="url(#clip-path)">
      <g id="Group_1" data-name="Group 1" transform="translate(-0.001)">
        <path id="Path_34" data-name="Path 34" d="M1156.16,328.468l-1618-2.95V-114.172S-468.545,49.16-11.408,44.283C586.761,37.9,423.038,252.227,733.419,166.171c254.986-70.692,422.741,162.3,422.741,162.3" transform="translate(461.842 114.172)" fill="#f5ba3b"/>
      </g>
    </g>
  </g>
</svg>
-->
