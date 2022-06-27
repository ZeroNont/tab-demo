<template>
<v-card color="#ffffff" class="file-content">
  <v-row>
    <v-col>
        <v-card outlined color="transparent" class="file-content">
            <h3>All Files</h3>
        <v-tabs
          v-model="model"
          centered
        >
        <v-tabs-slider color="#45a2db" style="margin-top: -10px;"></v-tabs-slider>
          <v-tab :key="Dates">
                    Date
                </v-tab>
                <v-tab :key="Name">
                    Name
                </v-tab>
                <v-tab :key="Type">
                    Type
                </v-tab>
        </v-tabs>
     <v-tabs-items v-model="file" class="tabs-items">
        <v-tab-item :key="Dates" class="custom-tab-items">
        1
        </v-tab-item>
        <v-tab-item :key="Name" class="custom-tab-items">
        2
        </v-tab-item>
         <v-tab-item :key="Type" class="custom-tab-items">
        3
        </v-tab-item>
        </v-tabs-items>
        </v-card>
    </v-col>
    <v-col>
        <v-card outlined color="transparent" class="file-content">
            <h3>Downloaded Files</h3>
        </v-card>
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
  padding: 20px;
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
.file-content{
  color: #000000 !important;
  padding: 20px;
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
