<template>
  <div>
    <!-- Hero -->
    <div class="bg-body-light">
      <div class="content content-full">
        <div class="d-flex flex-column flex-sm-row justify-content-sm-between align-items-sm-center py-2 text-center text-sm-left">
          <div class="flex-sm-fill">
            <h1 class="h3 font-w600 mb-2">
              Entnahme Kleinteileager für Auftrag XYZ, 12345, Jana und Jonas Jenke
            </h1>
          </div>
        </div>
      </div>
    </div>
    <!-- END Hero -->

    <!-- Page Content -->
    <div class="content">
      <!-- <base-block rounded>
      </base-block> -->
      <b-table-simple responsive striped table-class="table-vcenter">
        <b-thead>
          <b-tr>
            <b-th class="text-center" style="width: 70px;">Status</b-th>
            <b-th>Gepickt</b-th>
            <b-th>Menge</b-th>
            <b-th style="min-width: 180px;">Material</b-th>
            <b-th>Reihenfolge</b-th>
          </b-tr>
        </b-thead>
        <b-tbody>
          <b-tr v-for="user in users" :key="user.id">
            <b-td class="text-center">
              <b-badge :variant="user.labelVariant" class="statusDot">.</b-badge>
            </b-td>
            <b-td>
              {{ user.gepickt }}
            </b-td>
            <b-td class="font-size-sm">
              {{ user.menge }}
            </b-td>
            <b-td>
              {{ user.material }}
            </b-td>
            <b-td>
              {{ user.reihenfolge }}
            </b-td>
          </b-tr>
        </b-tbody>
      </b-table-simple>

      <div class="btmBtns mb-4">
        <b-form-row>
          <b-col cols="sm-auto" class="mt-3">
            <a href="javascript:void(0)" class="btn btn-primary w-100 btn-lg">Buchung beginnen</a>
          </b-col>
          <b-col cols="sm-auto" class="mt-3">
            <a href="javascript:void(0)" class="btn btn-success w-100 btn-lg">Buchung bestätigen</a>
          </b-col>
        </b-form-row>
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
          gepickt: '12',
          menge: '12',
          material: 'Schraube 30 mm, silber, #1234',
          labelVariant: 'success',
          reihenfolge: '1'
        },
        {
          id: 2,
          gepickt: '12',
          menge: '12',
          material: 'Schraube 20 mm, silber, #13234',
          labelVariant: 'success',
          reihenfolge: '2'
        },
        {
          id: 3,
          gepickt: '9',
          menge: '12',
          material: 'Schraube 60 mm, silber, #123879',
          labelVariant: 'danger',
          reihenfolge: '3'
        }
      ]
    }
  }
}
</script>
