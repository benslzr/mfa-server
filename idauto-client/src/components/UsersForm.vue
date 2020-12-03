<template>
<div>
  <b-card bg-variant="light">
    <b-form-group
      label-cols-lg="1"
      label="User"
      label-size="sm"
      label-class="font-weight-bold pt-0"
      class="mb-0"
    >
      <b-form-group
        label-cols-sm="5"
        label="Username:"
        label-align-sm="right"
        label-for="nested-username"
      >
        <b-form-input id="nested-username"></b-form-input>
      </b-form-group>

      <b-form-group
        label-cols-sm="3"
        label="Domain:"
        label-align-sm="right"
        label-for="nested-domain"
      >
        <b-form-input id="nested-domain"></b-form-input>
      </b-form-group>

      <b-form-group
        label-cols-sm="3"
        label="Email:"
        label-align-sm="right"
        label-for="nested-email"
      >
        <b-form-input id="nested-email"></b-form-input>
      </b-form-group>

      <b-form-group
        label-cols-sm="3"
        label="Mobile:"
        label-align-sm="right"
        label-for="nested-mobile"
      >
        <b-form-input id="nested-mobile"></b-form-input>
      </b-form-group>

      <b-form-group
        label-cols-sm="3"
        label="Buttons"
        label-align-sm="right" class="mb-0"
      >
  <div>
    <b-button-group>
      <b-button>Add</b-button>
      <b-button>Update</b-button>
      <b-button>Del</b-button>
    </b-button-group>
  </div>
      </b-form-group>
    </b-form-group>
  </b-card>
</div>
</template>

<script>
  export default {
    data() {
      return {
        items: [
          { age: 40, first_name: 'Dickerson', last_name: 'Macdonald' },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>