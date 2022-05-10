<template>
  <v-container
    transition="expand-x-transition"
    fluid
    class="d-flex flex-column justify-center align-center my-auto"
  >
    <v-col cols="6" class="d-flex flex-column justify-center">
      <v-img
        src="https://vaccineforthais.ais.th/Images/MicrosoftTeams-image.png"
      ></v-img>
      <div class="mx-auto mt-10">
        <h4 class="mb-1">บริการลงทะเบียนรับวัคซีนโควิด-19 โดย เอไอเอส</h4>
        <h4 class="mb-2 font-weight-light">
          จัดสรรโดย กรมการแพทย์ กระทรวงสาธารณสุข และกระทรวงคมนาคม
        </h4>

        <div>
          <h4 class="mb-1">บริการลงทะเบียนรับวัคซีนโควิด-19 โดย เอไอเอส</h4>
          <p class="mb-1 text-caption">เพื่อล็อกอินลงทะเบียนรับวัคซีน</p>
          <v-row class="mt-5">
            <v-text-field
              class="mr-5"
              dense
              solo
              placeholder="0XX-XXX-XXXX"
              data-val-regex-pattern="^\(?([0-9]{3})\)?[-. ]?([0-9]{3})[-. ]?([0-9]{4})$"
            ></v-text-field>
            <v-btn
              color="#8DC63F"
              style="color: white"
              @click="modalStatus = true"
              >รับรหัส OTP ทาง SMS</v-btn
            >
          </v-row>
        </div>

        <div v-if="modalStatus == true">
          <h4 class="mb-1">ระบุรหัส OTP ที่ได้รับทาง SMS</h4>
          <p class="mb-1 text-caption">(รหัสผ่านมีอายุการใช้งาน 5 นาที)</p>
          <v-row class="mt-5">
            <v-text-field
              class="mr-5"
              dense
              solo
              placeholder="XXXX"
            ></v-text-field>
            <v-btn color="#8DC63F" style="color: white">เข้าสู่ระบบ</v-btn>
          </v-row>
        </div>

        <h4 class="mb-1" style="color: #74a822">
          ข้อควรรู้ก่อนลงทะเบียนรับวัคซีน
        </h4>
        <ul>
          <b><li>กลุ่มอายุ 12-17 ปี</li></b
          >•&nbsp;รับวัคซีนเข็ม 3: ฉีด 2 เข็ม ครบ 120 วัน<br /><br /><b
            ><li>กลุ่มอายุ 18 ปี ขึ้นไป</li></b
          >•&nbsp;รับวัคซีนเข็ม 3: ฉีด 2 เข็ม ครบ 90 วัน<br />
          •&nbsp;รับวัคซีนเข็ม 4: ฉีด 3 เข็ม ครบ 120 วัน<br /><br /><b
            ><li>สถานที่: สถานีกลางบางซื่อ</li></b
          >
        </ul>
        <ul class="mt-5">
          <li>
            <b>รอรับ SMS แจ้งผลลงทะเบียนภายใน 2 ชม.</b>
          </li>
          <li>
            <b>1 หมายเลข (ค่ายใดก็ได้) / 5 บัตรประชาชน บัตรชมพู หรือพาสปอร์ต</b>
          </li>
        </ul>

        <div class="d-flex justify-center my-8">
          <v-btn class="mx-auto" color="#5c8e26" style="color: white"
            >ดูคำถามที่พบบ่อย</v-btn
          >
        </div>
      </div>
    </v-col>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      modalStatus: false,
    };
  },
};
</script>
