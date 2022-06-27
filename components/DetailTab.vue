<!-- Please remove this file from your project -->
<template>
 <v-card color="#ffffff" class="content">
       <v-row>
        <v-col class="text-title">
          ครั้งที่ประชุม
        </v-col>
        <v-col class="text-content">
          1
        </v-col>
       </v-row>
       <v-row>
        <v-col class="text-title">
          เวลา
        </v-col>
        <v-col class="text-content">
          14.00 - 15.30 (1.5 ชม.)
        </v-col>
       </v-row>
        <v-row>
        <v-col class="text-title">
          สถานที่
        </v-col>
        <v-col class="text-content">
          google meet
        </v-col>
       </v-row>
          <v-row>
        <v-col class="text-title">
          ลิงก์ (ถ้ามี)
        </v-col>
        <v-col class="text-link">
            <p><a href="https://www.google.co.th/?hl=th" target="_blank">https://www.google.co.th/?hl=th </a> </p> 
          
        </v-col>
       </v-row>
        <v-row>
        <v-col class="text-title">
          ผู้จัดการประชุม
        </v-col>
        <v-col class="text-content">
          Sophon
        </v-col>
       </v-row>
         <v-row>
        <v-col class="text-title">
          วาระการประชุม
        </v-col>
        <v-col class="text-content">
            <v-row>
                <v-col class="text-content">
                    1.ความคืบหน้าของงาน
                </v-col>
            </v-row>
            <v-row> 
                <v-col class="text-content">
                    2.ติดตามงาน
                </v-col>
               </v-row>
        </v-col>
       </v-row>
          <v-row>
        <v-col class="text-title">
          ดาวน์โหลด
        </v-col>
        <v-col class="text-content">
          อนุญาต
        </v-col>
       </v-row>
           <v-row>
        <v-col class="text-title">
          คำอธิบายเพิ่มเติม
        </v-col>
        <v-col class="text-content">
          -
        </v-col>
       </v-row>
            <v-row>
        <v-col class="text-title">
          แจ้งเตือน
        </v-col>
        <v-col class="text-content">
          12 ชั่วโมงก่อนถึงนัดหมาย
        </v-col>
       </v-row>
            <v-row>
        <v-col class="text-title">
          ประเภทการประชุม
        </v-col>
        <v-col class="text-content">
          การประชุมทั่วไป
        </v-col>
       </v-row>
           <v-row>
        <v-col class="text-title">
          ระเบียบวาระการประชุม
        </v-col>
        <v-col class="text-content">
          <v-btn
        class="ma-2"
        color="indigo"
        dark
      >
        <v-icon dark>
          mdi-file-pdf-box
        </v-icon>
      </v-btn>
        </v-col>
       </v-row>
      </v-card>
</template>
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
.main-tab{
  margin-top: 50px;
}
a{
    text-decoration: none;
}
.content{
  color: #000000 !important;
  padding: 50px;
  border-radius: 20px !important;
}
.text-title{
  max-width: 250px;
  font-weight: bold;
}
.text-link{
  font-weight: bold;
  color: #3feaff;
}
.text-content{
color: #00000099 !important;
}
.container{
  border-radius: 10px;
}
</style>
