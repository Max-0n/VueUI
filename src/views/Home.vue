<template lang="pug">
  .home
    .row.fixed
      .cell
        h2
          a(href="https://vuetifyjs.com/en/components/dialogs", target="_blank") Vuetify
      .cell
        h2
          a(href="https://vuematerial.io/components/dialog/", target="_blank") Material
      .cell
        h2
          a(href="https://bootstrap-vue.js.org/docs/components/alert", target="_blank") Bootstrap
      .cell
        h2
          a(href="https://element.eleme.io/#/en-US/component/notification", target="_blank") Element
    .row
      h3 Buttons
      .cell
        img(src="../assets/vuetify/buttons_1.gif")
        img(src="../assets/vuetify/buttons_2.gif")
        img(src="../assets/vuetify/buttons_3.gif")
      .cell
        img(src="../assets/material/buttons.gif")
      .cell
        img(src="../assets/bootstrap/buttons.gif")
      .cell
        img(src="../assets/elements/buttons.gif")
    .row
      h3 Inputs
      .cell
        img(src="../assets/vuetify/inputs.gif")
        img(src="../assets/vuetify/inputs_2.gif")
        img(src="../assets/vuetify/inputs_3.gif")
      .cell
        img(src="../assets/material/inputs.gif")
      .cell
        img(src="../assets/bootstrap/inputs.gif")
      .cell
        img(src="../assets/elements/inputs_1.gif")
        img(src="../assets/elements/inputs_2.gif")
        img(src="../assets/elements/inputs_number.gif")
    .row
      h3 Selects
      .cell
        img(src="../assets/vuetify/selects_1.gif")
        img(src="../assets/vuetify/selects_2.gif")
      .cell
        img(src="../assets/material/selects.gif")
      .cell
        img(src="../assets/bootstrap/selects.gif")
      .cell
        img(src="../assets/elements/selects_1.gif")
        img(src="../assets/elements/selects_2.gif")
        //- img(src="../assets/elements/selects_3.gif")
    .row
      h3 Datepicker
      .cell
        img(src="../assets/vuetify/datepicker.gif")
      .cell
        img(src="../assets/material/datepicker.gif")
      .cell No
      .cell
        img(src="../assets/elements/datepicker.gif")
    .row
      h3 Checkboxes & Radio
      .cell
        img(src="../assets/vuetify/checkbox.gif")
      .cell
        img(src="../assets/material/checkbox_1.gif")
        img(src="../assets/material/checkbox_2.gif")
      .cell
        img(src="../assets/bootstrap/checkbox_1.gif")
        img(src="../assets/bootstrap/checkbox_2.gif")
      .cell
        img(src="../assets/elements/checkboxes_1.gif")
        img(src="../assets/elements/checkboxes_2.gif")
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({})
export default class Home extends Vue {}
</script>

<style scoped lang="scss">
h2 {
  font-weight: lighter;
  font-size: 30px;
  a {
    display: inline-block;
    position: relative;
    text-decoration: none;
    color: inherit;
    transition: all .2s ease-in-out;
    &:hover {
      color: rgb(70,70,200);
    }
  }
}

h3 {
  margin: auto;
  padding: 15px 0;
  border: 1px solid rgba(0,0,0,.1);
  border-left: none;
  border-right: none;
}
.home {
  text-align: center;
  padding-top: 101px;
}

.row {
  display: block;
  margin: auto;
  padding-bottom: 50px;
  &.fixed {
    position: fixed;
    top: 0; right: 0; left: 0;
    padding: 0;
    background: rgba(241,242,243,.9);
    box-shadow: 0px 1px 2px rgba(0,0,0,.075);
    z-index: 10;
  }
  .cell {
    display: inline-block;
    width: 350px;
    padding: 5px 10px;
    vertical-align: middle;
    // &:nth-child(1) { background: rgba(0,0,0,.1); }
    // &:nth-child(2) { background: rgba(0,0,0,.14); }
    // &:nth-child(3) { background: rgba(0,0,0,.1); }
    img {
      max-width: 100%;
      height: auto;
      transition: all 200ms ease-in-out;
      &:hover {
        transform: scale(1.1);
      }
    }
  }
}
</style>
