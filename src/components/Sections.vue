<template>
  <div class="main-divs">
    <!-- <navbar></navbar> -->
    <mdb-view class="back position-absolute">
      <img src="../assets/imgs/laptop.jpg" class="img-fluid w-100" alt="test" />
      <mdb-mask flex-center overlay="black-light" />
    </mdb-view>

    <div class="text-1 text-white">
      <mdb-row>
        <mdb-col md="6" offsetMd="3" class="text-overlay">
          <span class="display-4">WELCOME TO UBYTE</span>
          <p>
            APLICATIVO MÓVEL PARA
            <span class="highlight">DESIGNERS</span>, SOFTWARES PARA
            <span class="highlight">DESENVOLVEDORES</span>
          </p>
          <mdb-btn outline="white" size="lg">Conheça nossas soluções</mdb-btn>
        </mdb-col>
      </mdb-row>
    </div>
  </div>
</template>

<script>
import { mdbMask, mdbView, mdbBtn, mdbRow, mdbCol } from "mdbvue";
export default {
  components: { mdbMask, mdbView, mdbBtn, mdbRow, mdbCol }
};
</script>

<style lang="scss" scoped>
@import "../scss/variables";
.main-divs,
.background,
.overlay {
  height: 100vh;
  -ms-height: 100vh;
  -moz-height: 100vh;
  -webkit-height: 100vh;
  
  width: 100vw;
  -ms-width: 100vw;
  -moz-width: 100vw;
  -webkit-width: 100vw;
}

img {
  object-fit: cover;
  -ms-object-fit: cover;
  -moz-object-fit: cover;
  -webkit-object-fit: cover;
}
.back {
  z-index: -1;
  -ms-z-index: -1;
  -moz-z-index: -1;
  -webkit-z-index: -1;
}

.text-1 {
  z-index: 1;
  -ms-z-index: 1;
  -moz-z-index: 1;
  -webkit-z-index: 1;
  .text-overlay {
    margin-top: 20%;
    -ms-margin-top: 20%;
    -moz-margin-top: 20%;
    -webkit-margin-top: 20%;
  }
}
.highlight {
  color: $highlightColor;
  -ms-color: $highlightColor;
  -moz-color: $highlightColor;
  -webkit-color: $highlightColor;
}
</style>