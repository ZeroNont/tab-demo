<!-- Please remove this file from your project -->
<template>
<div>

 <v-card color="#ffffff" class="content">
       <v-row>
        <v-col class="text-title" sm="4">
          ครั้งที่ประชุม
        </v-col>
        <v-col class="text-content" sm="8">
    <v-text-field  v-model="number" placeholder="1"  outlined  dense   ></v-text-field>
        </v-col>
          <v-col class="text-right">
           <a href="/">
<v-icon
      large
      color="#0b499c"
    >
      mdi-cog-outline
    </v-icon>
           </a>

           
      </v-col>
       </v-row>
       <v-row>
        <v-col class="text-title">
          เวลา
        </v-col>
        <v-col class="text-content" sm="8">
          <v-text-field  v-model="time"   placeholder="14.00 - 15.30 (1.5 ชม.)"  outlined  dense   ></v-text-field>
        </v-col>
       </v-row>
        <v-row>
        <v-col class="text-title">
          สถานที่
        </v-col>
        <v-col class="text-content" sm="8">
          <v-text-field  v-model="location"   placeholder="Google Meet"  outlined  dense   ></v-text-field>
        </v-col>
       </v-row>
          <v-row>
        <v-col class="text-title">
          ลิงก์ (ถ้ามี)
        </v-col>
        <v-col class="text-link" sm="8">
          <v-text-field  v-model="link"   placeholder="https://www.google.co.th/?hl=th"  outlined  dense   ></v-text-field>
        </v-col>
       </v-row>
        <v-row>
        <v-col class="text-title">
          ผู้จัดการประชุม
        </v-col>
        <v-col class="text-content" sm="8">
            <v-text-field  v-model="manager"   placeholder="Sophon"  outlined  dense   ></v-text-field>
        </v-col>
       </v-row>
         <v-row>
        <v-col class="text-title" sm="4">
          วาระการประชุม
        </v-col>
        <v-col class="text-content" sm="8">
            <v-text-field  v-model="proposal"   placeholder="1.ความคืบหน้าของาน"  outlined  dense   ></v-text-field>
        </v-col>
        <v-col class="text-left">
          <a>
            <v-icon
      large
      color="#0b499c"
    >
      mdi-plus-circle
    </v-icon>
          </a>
        </v-col>
       </v-row>
          <v-row>
        <v-col class="text-title">
          ดาวน์โหลด
        </v-col>
        <v-col class="text-content" sm="8">
           <v-radio-group
      v-model="row"
      row
    >
      <v-radio
        label="อนุญาต"
        value="radio-1"
      ></v-radio>
      <v-radio
        label="ไม่อนุญาต"
        value="radio-2"
      ></v-radio>
    </v-radio-group>
        </v-col>
       </v-row>
           <v-row>
        <v-col class="text-title">
          คำอธิบายเพิ่มเติม
        </v-col>
        <v-col class="text-content" sm="8">
          <v-text-field  v-model="description"   placeholder="-"  outlined  dense   ></v-text-field>
        </v-col>
       </v-row>
            <v-row>
        <v-col class="text-title">
          แจ้งเตือน
        </v-col>
        <v-col class="text-content" sm="3">
               <v-overflow-btn
          class="my-2"
          :items="dropdownItems"
          label="การแจ้งเตือน"
          item-value="text"
          dense
        ></v-overflow-btn>
        </v-col>
       </v-row>
            <v-row>
        <v-col class="text-title">
          ประเภทการประชุม
        </v-col>
        <v-col class="text-content" sm="3">
          <v-overflow-btn
          class="my-2"
          :items="Items"
          label="ประเภทการประชุม"
          item-value="text"
          dense
        ></v-overflow-btn>
        </v-col>
       </v-row>
           <v-row>
        <v-col class="text-title">
          ระเบียบวาระการประชุม
        </v-col>
        <v-col class="text-content" sm="3">
         <v-file-input
  truncate-length="15"
></v-file-input>
        </v-col>
       </v-row>
      </v-card>
      <v-row>
        <v-col  class="text-right"> <v-btn
                        color="#0b499c"
                        height="32px"
                        dark
                        depressed
                        class=""
                        >บันทึก</v-btn
                    ></v-col>
      </v-row>
        
</div>
</template>
<script>
export default {
  name: "Insert",
  data: () => ({
    dropdownItems: [{ text: "8 ชั่วโมง ก่อนถึงเวลานัดหมาย" }, { text: "10 ชั่วโมง ก่อนถึงเวลานัดหมาย" }, { text: "12 ชั่วโมง ก่อนถึงเวลานัดหมาย" }],
    Items: [{text:'การประชุมทั่วไป'},{text:'การประชุมเพิ่มเติม'},{text:'การประชุมลับ'}],
  }),
};
</script>
<style>
.v-input__control {
    display: flex;
    flex-direction: column;
    height: 20px;
    flex-grow: 1;
    flex-wrap: wrap;
    min-width: 0;
    width: 100%;
}
.main{
  padding: 50px !important;
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
  padding: 50px !important;
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
