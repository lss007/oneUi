<template>
  <div>
    <!-- Hero -->
    <div class="bg-body-light">
      <div class="content content-full">
        <div class="d-flex flex-column flex-sm-row justify-content-sm-between align-items-sm-center py-2 text-center text-sm-left">
          <div class="flex-sm-fill">
            <h1 class="h3 font-w600 mb-2">
              Angebot "1000 " ansehen
            </h1>
          </div>
          <div class="mt-3 mt-sm-0 ml-sm-3">
            <b-breadcrumb class="breadcrumb-alt">
              <b-breadcrumb-item href="javascript:void(0)">Angebotverwaltung</b-breadcrumb-item>
              <b-breadcrumb-item active>Angebot "1000 " ansehen</b-breadcrumb-item>
            </b-breadcrumb>
          </div>
        </div>
      </div>
    </div>
    <!-- END Hero -->

    <!-- Page Content -->
    <div class="content">
      <div class="topRightOptions">
        <b-row class="justify-content-end mb-3">
          <b-col cols="auto">
            <ul class="optionLinks">
              <li><a title="" target="" href="javascript:void(0)" class="btn btn-info" data-toggle="tooltip" data-html="true" data-placement="top" data-title="&quot;1000 &quot; bearbeiten" data-original-title=""><i class="ace-icon fa fa-pencil-alt"></i></a></li>
              <li><a title="" target="" href="javascript:void(0)" class="btn btn-danger confirmation-box-link" data-toggle="tooltip" data-html="true" data-placement="top" data-title="&quot;1000 &quot; löschen" data-confirmation="Soll Angebot &quot;1000 &quot; wirklich gelöscht werden?" data-confirmation-ok="Ok" data-confirmation-cancel="Abbrechen" data-original-title=""><i class="ace-icon fa fa-trash"></i></a></li>
              <li><a title="" target="" href="javascript:void(0)" class="btn btn-secondary" data-toggle="tooltip" data-html="true" data-placement="top" data-title="Aktivität zu &quot;1000 &quot; anzeigen" data-original-title=""><i class="ace-icon fa fa-history"></i></a></li>
              <li><a title="" target="" href="javascript:void(0)" class="btn btn-success" data-toggle="tooltip" data-html="true" data-placement="top" data-title="Copy" data-original-title=""><i class="ace-icon fa fa-copy"></i></a></li>
              <li>
                <b-dropdown id="dropdown-right" right  variant="success">
                  <template #button-content>
                    <i class="ace-icon fa fa-plus"></i>
                  </template>
                  <b-dropdown-item href="#"><i class="ace-icon far fa-file-pdf"></i> Angebotsdateien erstellen</b-dropdown-item>
                  <b-dropdown-item href="#"><i class="ace-icon fa fa-align-right"></i> Angebotsposition Dienstleistung erstellen</b-dropdown-item>
                  <b-dropdown-item href="#"><i class="ace-icon fa fa-align-right"></i> Angebotsposition Artikel erstellen</b-dropdown-item>
                  <b-dropdown-item href="#"><i class="ace-icon fa fa-cut"></i> Artikelposition Schnittware erstellen</b-dropdown-item>
                </b-dropdown>
              </li>
            </ul>
          </b-col>
        </b-row>
      </div>
      <div class="tabContent">
        <!-- Block Tabs Animated Fade -->
        <b-tabs class="block" nav-class="nav-tabs-block" content-class="block-content overflow-hidden">
          <b-tab>
            <template #title>
              <span class="tabLinkIcon"><i class="fa fa-info-circle"></i></span> <span class="tabLinkText">Details</span>
            </template>
            <p class="p-3">Tab contents 1</p>
          </b-tab>
          <b-tab>
            <template #title>
              <span class="tabLinkIcon"><i class="fa fa-align-right"></i></span> <span class="tabLinkText">Angebotspositionen</span> <b-badge variant="dark">2</b-badge>
            </template>
            <p class="p-3">Tab contents 2</p>
          </b-tab>
          <b-tab>
            <template #title>
              <span class="tabLinkIcon"><i class="fa fa-file-pdf-o"></i></span> <span class="tabLinkText">Angebotsdateiens</span> <b-badge variant="dark">0</b-badge>
            </template>
            <p class="p-3">Tab contents 3</p>
          </b-tab>
          <b-tab>
            <template #title>
              <span class="tabLinkIcon"><i class="fa fa-archive"></i></span> <span class="tabLinkText">Angebotshistories</span> <b-badge variant="dark">2</b-badge>
            </template>
            <p class="p-3">Tab contents 5</p>
          </b-tab>
          <b-tab>
            <template #title>
              <span class="tabLinkIcon"><i class="fa fa-align-right"></i></span> <span class="tabLinkText">Angebotsposition Dienstleistungs</span> <b-badge variant="dark">0</b-badge>
            </template>
            <p class="p-3">Tab contents 4</p>
          </b-tab>
          <b-tab>
            <template #title>
              <span class="tabLinkIcon"><i class="fa fa-align-right"></i></span> <span class="tabLinkText">Angebotsposition Artikels</span> <b-badge variant="dark">0</b-badge>
            </template>
            <p class="p-3">Tab contents 6</p>
          </b-tab>
          <b-tab>
            <template #title>
              <span class="tabLinkIcon"><i class="fa fa-cut"></i></span> <span class="tabLinkText">Artikelposition Schnittwares</span> <b-badge variant="dark">0</b-badge>
            </template>
            <p class="p-3">Tab contents 7</p>
          </b-tab>
          <b-tab active>
            <template #title>
              <span class="tabLinkIcon"><i class="far fa-file"></i></span> <span class="tabLinkText">Angebot</span>
            </template>
            <b-form>
              <h2 class="content-headingLg border-bottom mb-2 pb-2">Stammdaten</h2>
              <h4 class="content-heading border-bottom mb-4 pb-2">Kontakatinformationen</h4>
              <b-row>
                <b-col lg="6">
                  <b-form-group label="Kunde" label-for="fld1">
                    <b-form-input id="fld1" placeholder="Kunde" value="Herr Testkunde für Classic"></b-form-input>
                  </b-form-group>
                </b-col>
                <b-col lg="6">
                  <b-form-group label="Lieferadresse">
                    <v-select v-model="vSelectOptionsSelected" :options="vSelectOptionsMultiple" placeholder="Choose a value.."></v-select>
                  </b-form-group>
                </b-col>
                <b-col lg="6">
                  <b-form-group label="Postadresse">
                    <v-select v-model="postOptionsSelected" :options="postOptions" placeholder="Choose a value.."></v-select>
                  </b-form-group>
                </b-col>
                <b-col lg="6">
                  <b-form-group label="Rechnungsadresse">
                    <v-select v-model="billingAddressSelected" :options="billingAddress" placeholder="Choose a value.."></v-select>
                  </b-form-group>
                </b-col>
              </b-row>
              <h4 class="content-heading border-bottom mb-4 pb-2">Info</h4>
              <b-row>
                <b-col lg="6">
                  <b-form-group label="Titel" label-for="titleFld">
                    <b-form-input id="titleFld" placeholder="Title" value=""></b-form-input>
                  </b-form-group>
                </b-col>
                <b-col lg="6">
                  <b-form-group label="Angebotsnummer" label-for="oerderNoFld">
                    <b-form-input id="oerderNoFld" placeholder="Angebotsnummer" value="1000"></b-form-input>
                  </b-form-group>
                </b-col>
                <b-col lg="6">
                  <b-form-group label="Datum" label-for="dateFld">
                    <b-form-input id="dateFld" placeholder="Date" value="15-10-2019"></b-form-input>
                  </b-form-group>
                </b-col>
                <b-col lg="6">
                  <b-form-group label="Mitarbeiter">
                    <v-select v-model="employeOptionsSelected" :options="employeOptions" placeholder="Choose a value.."></v-select>
                  </b-form-group>
                </b-col>
                <b-col lg="6">
                  <b-form-group label="Status">
                    <v-select v-model="statusOptionsSelected" :options="statusOptions" placeholder="Choose a value.."></v-select>
                  </b-form-group>
                </b-col>
              </b-row>
              <h4 class="content-heading border-bottom mb-4 pb-2">Kopfzeile</h4>
              <b-form-group>
                <b-form-textarea id="textareaFld1" rows="4" placeholder="Textarea content.."></b-form-textarea>
              </b-form-group>
              <h4 class="content-heading border-bottom mb-4 pb-2">Angebotspositionen</h4>
              <b-table-simple responsive striped table-class="table-vcenter">
                <b-thead>
                  <b-tr>
                    <b-th>
                      Position
                    </b-th>
                    <b-th>Name</b-th>
                    <b-th>Menge</b-th>
                    <b-th>Einzelpreis</b-th>
                    <b-th>Rabatt</b-th>
                    <b-th>UST</b-th>
                    <b-th>Gesamtpreis</b-th>
                    <b-th></b-th>
                  </b-tr>
                </b-thead>
                <b-tbody>
                  <b-tr>
                    <b-td colspan="8">
                      <span class="mdTitle">elements </span>
                      <span class="plusIconDD">
                        <b-dropdown id="dropdown-right" right  variant="success">
                          <template #button-content>
                            <i class="ace-icon fa fa-plus"></i>
                          </template>
                          <b-dropdown-item href="#">Items</b-dropdown-item>
                          <b-dropdown-item href="#">Subtotal</b-dropdown-item>
                          <b-dropdown-item href="#">Heading</b-dropdown-item>
                        </b-dropdown>
                      </span>
                    </b-td>
                  </b-tr>
                  <b-tr>
                    <b-td>
                    </b-td>
                    <b-td>1 Zaunfeld Modell Berlin</b-td>
                    <b-td>
                      <b-input-group append="lfm">
                        <b-form-input type="text" value="2.37"></b-form-input>
                      </b-input-group>
                    </b-td>
                    <b-td>
                      <b-input-group append="EUR">
                        <b-form-input type="text" value="178.78"></b-form-input>
                      </b-input-group>
                    </b-td>
                    <b-td>
                      <b-input-group append="%">
                        <b-form-input type="text" value="0"></b-form-input>
                      </b-input-group>
                    </b-td>
                    <b-td>
                      <b-input-group append="%">
                        <b-form-input type="text" value="16"></b-form-input>
                      </b-input-group>
                    </b-td>
                    <b-td>
                      <b-input-group append="EUR">
                        <b-form-input type="text" value="24.33" disabled></b-form-input>
                      </b-input-group>
                    </b-td>
                    <b-td class="text-center">
                      <b-btn-group>
                        <b-button size="sm" variant="alt-primary">
                          <i class="fa fa-fw fa-pencil-alt"></i>
                        </b-button>
                        <b-button size="sm" variant="alt-primary">
                          <i class="fa fa-fw fa-plus"></i>
                        </b-button>
                        <b-button size="sm" variant="alt-primary">
                          <i class="far fa-fw fa-file"></i>
                        </b-button>
                        <b-button size="sm" variant="alt-primary">
                          <i class="far fa-fw fa-trash-alt"></i>
                        </b-button>
                      </b-btn-group>
                    </b-td>
                  </b-tr>
                </b-tbody>
              </b-table-simple>
            </b-form>
          </b-tab>
        </b-tabs>
        <!-- END Block Tabs Animated Fade -->
      </div>
    </div>
    <!-- END Page Content -->
  </div>
</template>

<style lang="scss">
// Vue Select + Custom overrides
@import '~vue-select/src/scss/vue-select';
@import './src/assets/scss/vendor/vue-select';
</style>

<script>
// Vue Select, for more info and examples you can check out https://github.com/sagalbot/vue-select
import VueSelect from 'vue-select'

export default {
  components: {
    'v-select': VueSelect,
  },
  data () {
    return {
      // Vue Select initial values
      vSelectOptionsMultiple: ['Building road Salzburg', 'Universalstrasse Salzburg', 'Stromberger Strasse 61 Weiler / Bingen'],
      vSelectOptionsMultipleSelected: null,
      postOptions: ['Mozartstrasse Salzburg', 'Option 2'],
      postOptionsSelected: null,
      billingAddress: ['Money Street Salzburg', 'Option 2'],
      billingAddressSelected: null,
      employeOptions: ['Herr Oliver Kreusel', 'Option 2'],
      employeOptionsSelected: null,
      statusOptions: ['angenommen', 'Option 2'],
      statusOptionsSelected: null,

    }
  }
}
</script>
