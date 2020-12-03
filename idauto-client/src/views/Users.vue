<template>
  <div>
<b-container class="user-mang-row">
  <b-row>
    <b-col><users-form></users-form></b-col>
    <b-col><users-table></users-table></b-col>
  </b-row>
    </b-container>
  </div>
</template>
<script>
import  UsersTable from "@/components/UsersTable.vue"
import  UsersForm from "@/components/UsersForm.vue"

export default {
  name: "Home",
  components: {
    "users-table": UsersTable,
    "users-form":UsersForm
    },
    data() {
    return {
      todos: [
        {
          id: 1,
          title: "Benjamin Salazar",
          completed: false
        },
        {
          id: 2,
          title: "Howard Cole",
          completed: true
        }
      ]
    }
  }
    
};
</script>
<style lang="scss" scoped>

.user-mang-row{
  background: white;
  margin: 10px;
  padding: 10px;
}

</style>
