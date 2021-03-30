<template>
  <div>
    <!-- Hero -->
    <div class="bg-body-light">
      <div class="content content-full">
        <div class="d-flex flex-column flex-sm-row justify-content-sm-between align-items-sm-center py-2 text-center text-sm-left">
          <div class="flex-sm-fill">
            <h1 class="h3 font-w600 mb-2">
              Erwartete Wareneingänge
            </h1>
          </div>
        </div>
      </div>
    </div>
    <!-- END Hero -->

    <!-- Page Content -->
    <div class="content">
      <div class="ewContent">
        <!-- <base-block rounded>
        </base-block> -->
        <b-form-row class="justify-content-end">
          <b-col cols="auto" class="mb-3">
            <a href="javascript:void(0)" class="btn btn-primary minWdBtn">Neu</a>
          </b-col>
          <b-col cols="auto" class="mb-3">
            <a href="javascript:void(0)" class="btn btn-success minWdBtn">...</a>
          </b-col>
          <b-col cols="sm-auto" class="mb-3">
            <b-form-input id="searchFld" placeholder="Search"></b-form-input>
          </b-col>
        </b-form-row>
        <b-form-row class="justify-content-end">
        </b-form-row>
        <b-table-simple responsive striped table-class="table-vcenter thNowrap">
          <b-thead>
            <b-tr>
              <b-th>Menge</b-th>
              <b-th>Was</b-th>
              <b-th>Artikel-Nr</b-th>
              <b-th>Art</b-th>
              <b-th>Lieferant</b-th>
              <b-th>Wann</b-th>
              <b-th>Ziellager</b-th>
              <b-th>Aktion</b-th>
            </b-tr>
          </b-thead>
          <b-tbody>
            <b-tr v-for="user in users" :key="user.id">
              <b-td class="text-center">{{ user.menge }}</b-td>
              <b-td>{{ user.was }}</b-td>
              <b-td>{{ user.artikel }}</b-td>
              <b-td>{{ user.art }}</b-td>
              <b-td>{{ user.liefereant }}</b-td>
              <b-td>{{ user.wann }}</b-td>
              <b-td>{{ user.ziellager }}</b-td>
              <b-td>
                <b-btn-group>
                  <b-form-checkbox class="custom-control-success align-self-center" value="success"></b-form-checkbox>
                  <b-button size="sm" variant="alt-info">
                    <i class="fa fa-fw fa-pencil-alt"></i>
                  </b-button>
                  <b-button size="sm" variant="alt-warning">
                    <i class="fa fa-print"></i>
                  </b-button>
                </b-btn-group>
              </b-td>
            </b-tr>
          </b-tbody>
        </b-table-simple>
      </div>

    </div>
    <!-- END Page Content -->
  </div>
</template>

<script>
export default {
  data () {
    return {
      users: [
        {
          id: 1,
          menge: '4000',
          was: 'Schrauben 30mm',
          artikel: '789123',
          art: 'Bestellung #4711',
          liefereant: 'Motorenwerke',
          wann: '28.12.2020',
          ziellager: 'G2R23F45'
        },
        {
          id: 2,
          menge: '3',
          was: 'Motor 220V',
          artikel: '896612',
          art: 'Retoure aus Auftrag #98754',
          liefereant: 'Elon Musk',
          wann: '14.02.2021',
          ziellager: 'G82R24F43'
        },
        {
          id: 3,
          menge: '7',
          was: '6m-Querstangen',
          artikel: '789123',
          art: 'Beschichtungsauftrag #1235',
          liefereant: 'Hermann Schwenk',
          wann: '28.01.2020',
          ziellager: 'G82R24F4'
        }
      ]
    }
  }
}
</script>
