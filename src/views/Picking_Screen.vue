<template>
  <div>
    <!-- Hero -->
    <div class="bg-body-light">
      <div class="content content-full">
        <div class="d-flex flex-column flex-sm-row justify-content-sm-between align-items-sm-center py-2 text-center text-sm-left">
          <div class="flex-sm-fill">
            <h1 class="h3 font-w600 mb-2">
            Pick für
            </h1>
          </div>
        </div>
      </div>
    </div>
    <!-- END Hero -->

    <!-- Page Content -->
    <div class="content">
      <div class="pickingScreen">
        <b-row>
          <b-col cols="sm-auto" class="order-sm-last">
            <img class="proImg1" :src="`img/img-1.png`" alt="img">
          </b-col>
          <b-col cols="sm">
            <h4 class="mdTitle mb-2 text-warning">40 Stück</h4>
            <h4 class="mdTitle mb-2">Schraube 30mm, #1234532</h4>
            <p class="mb-2">Gang 3 Regal 4 Fach 5</p>
            <span>Pick 3/10</span>
          </b-col>
        </b-row>
        <div class="btmBtns mb-4">
          <b-form-row>
            <b-col cols="sm-auto" class="mt-3">
              <a href="javascript:void(0)" class="btn btn-secondary w-100 btn-lg">zu vorherigen Artikel</a>
            </b-col>
            <b-col cols="sm-auto" class="mt-3"><a href="javascript:void(0)" class="btn btn-primary w-100 btn-lg">Ändern</a></b-col>
            <b-col cols="sm-auto" class="mt-3">
              <a href="javascript:void(0)" class="btn btn-success w-100 btn-lg">Buchung bestätigen</a>
            </b-col>
          </b-form-row>
        </div>
        <p>Nächster Pick: 23 x Mutter grün  #12345 Gang 4 Regal 32 Fach 4</p>
      </div>
    </div>
    <!-- END Page Content -->
  </div>
</template>
