<template>
  <div>
    <!-- Hero -->
    <div class="bg-body-light">
      <div class="content content-full">
        <div class="d-flex flex-column flex-sm-row justify-content-sm-between align-items-sm-center py-2 text-center text-sm-left">
          <div class="flex-sm-fill">
            <h1 class="h3 font-w600 mb-2">
              Inventurscan
            </h1>
          </div>
        </div>
      </div>
    </div>
    <!-- END Hero -->

    <!-- Page Content -->
    <div class="content">
      <div class="inventurscanScreen">
        <b-row>
          <b-col cols="sm-auto" class="order-sm-last">
            <div class="scanRightImgCol">
              <img class="scanImg" :src="`img/img-2.png`" alt="img">
            </div>
          </b-col>
          <b-col cols="sm">
            <b-form>
              <b-form-group label="Lagerplatz" label-for="lagerplatzFld">
                <b-form-input id="lagerplatzFld" placeholder="Text Input"></b-form-input>
              </b-form-group>
              <b-form-group label="Artikel" label-for="artikelFld">
                <b-form-input id="artikelFld" placeholder="Text Input"></b-form-input>
              </b-form-group>
              <b-form-group label="Menge" label-for="mengeFld">
                <b-form-input id="mengeFld" placeholder="Text Input"></b-form-input>
              </b-form-group>
              <b-button variant="success" class="minWdBtn btn-lg">SCAN</b-button>
            </b-form>
          </b-col>
        </b-row>
      </div>

    </div>
    <!-- END Page Content -->
  </div>
</template>
