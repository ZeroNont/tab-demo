<template>
 <div class="main">
  <v-row>
    <v-col>
<h2 class="topic">ประชุมผู้บริหาร B</h2>
    </v-col>
    <v-col class="text-right">
         <v-btn 
                        color="#e8f6fc"
                        height="32px"
                        dark
                        depressed
                        border-color="#0b499c"
                        class="btn-sumary"
                        >สรุปการประชุม</v-btn
                    >
       <v-btn
                        color="#0b499c"
                        height="32px"
                        dark
                        depressed
                        class=""
                        >เข้าร่วม</v-btn
                    >
    </v-col>
  </v-row>

<p style="color:#a6b1b6;">14 january 2022</p>
<div class="main-tab">
   <v-tabs  style="background: transparent;" v-model="tab" align-with-title>
            <v-tabs-slider color="#45a2db" style="margin-top: -10px;"></v-tabs-slider>

           <v-tab :key="Detail">
                    Details
                </v-tab>
                <v-tab :key="Member">
                    Member
                </v-tab>
                <v-tab :key="Files">
                    Files
                </v-tab>
    </v-tabs>
        <v-tabs-items v-model="tab" class="tabs-items">
        <v-tab-item :key="Detail" class="custom-tab-items">
        <DetailTab/>
        </v-tab-item>
        <v-tab-item :key="Member" class="custom-tab-items">
        <MemberTab/>
        </v-tab-item>
         <v-tab-item :key="Files" class="custom-tab-items">
        <FileTab/>
        </v-tab-item>
        </v-tabs-items>
        </div>
 </div>
</template>

<script>
import NuxtLogo from '~/components/NuxtLogo.vue';
import DetailTab from '../components/DetailTab.vue';
import MemberTab from '../components/MemberTab.vue';
import FileTab from '~/components/FileTab.vue';
export default {
    name: "IndexPage",
    components: { NuxtLogo, DetailTab, MemberTab, FileTab },
    data() {
    return {
      tab: null,
      items: ['Detail','Member','Files'],
    };
  },
}
</script>
<style>
.v-main__wrap{
  background-color: #e8f6fc;
}
.container{
  background-color: #e8f6fc;
}
.tabs-items{
  margin-top: 20px;
}
.main{
  padding: 50px;
}
.btn-sumary {
  border: thin solid #0b499c !important ;
  color: #0b499c !important;
}
.main-tab{
  margin-top: 20px;
}
.content{
  color: #000000 !important;
  padding: 50px;
}
.text-title{
  max-width: 250px;
  font-weight: bold;
}
.text-link{
  font-weight: bold;
  color: #3feaff;
}
.v-tab{
  color: #00000099 ;
  margin-left: 0px !important;
  text-transform: none !important;
}
.v-tab--active{
  color: #000000 !important;
}
.primary--text {
    color: #000000 !important;
    caret-color: #000000 !important;
    background-color: transparent !important;
}
.custom-tab-items {
   background-color: #e8f6fc !important;
}
</style>