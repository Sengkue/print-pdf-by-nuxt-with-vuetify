<template>
  <div>
    <h1>My Printable Content</h1>
    <div id="printMe" class="d-flex justity-center" >
      <v-card class="mt-5" max-with="500">
        <v-card-tittle>chily store</v-card-tittle>
        <v-card-text>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem nobis magnam voluptatem deserunt, voluptatum rerum odio amet doloremque, veniam dolorem illum et eligendi in nemo! Quaerat praesentium eligendi non sit!
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorum numquam officiis neque facere quaerat. Commodi odit, eius sequi quis illo illum, debitis, aperiam sint impedit expedita molestiae eveniet assumenda culpa!
          <p>This content will be printed.</p>
        </v-card-text>
      </v-card>
    </div>
    <v-btn class="mt-5 pt-5" @click="print">Print</v-btn>
  </div>
</template>

<script>
export default {
layout:'blank',
  methods: {
    print() {
      this.$htmlToPaper('printMe');
    }
  }
}
</script>
