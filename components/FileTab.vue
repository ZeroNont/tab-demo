<template>
<v-card color="#ffffff" class="content">
  <v-row>
    <v-col>
        <v-card color="transparent !important" class="content"></v-card>
    </v-col>
    <v-col>
        <v-card color="#ffffff" class="content"></v-card>
    </v-col>
  </v-row>
</v-card>
</template>  
<script>
  export default {
    data: () => ({
    }),
  }
</script>
<style>
.main{
  padding: 50px;
}
.btn-sumary {
  border: thin solid #0b499c !important ;
  color: #0b499c !important;
}
.theme--dark.v-application {
    background: #e8f6fc;
    color: #000000;
}
.elevation-1{
   background-color: #ffffff !important; 
  color: #000000 !important; 
  border-radius: 10px!important;
}
.content{
  color: #000000 !important;
}
.text-title{
  max-width: 250px;
  font-weight: bold;
}
.text-link{
  font-weight: bold;
  color: #3feaff;
}
.theme--dark.v-data-table > .v-data-table__wrapper > table > thead > tr > th {
    color: #ffffff;
    background-color: #0b499c;
}
</style>
