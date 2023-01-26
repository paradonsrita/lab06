<script setup >
import {ref} from "vue";

const stuID=ref("");
const stuName=ref("");
const phoneNumber=ref("");
const course=ref("");
const group=ref("");
const branch=ref("");
const newName=ref("");
const newLastname=ref("");
</script>


<template>
  <center>
  <h1>คําร้องขอเปลี่ยนชื่อ - นามสกุล</h1>
  </center>
  <br><form>
    <br>
    วันที่ <input type="date" name="" id="" >
    <br>
    <h4>เรื่อง ขอเปลี่ยนชื่อ - นามสกุล</h4>
    <h4>เรียน หัวหน้างานกลุ่มภารกิจทะเบียนเรียน ประมวลผล และรับเข้า</h4>
    <br>
    รหัสนักศึกษา <input type="" v-model="stuID" name="" id="" required >
    ชื่อ <input type="text" v-model="stuName" name="" id="" maxlength="100" required>
    <br>หมายเลขโทรศัพท์ <input type="text" v-model="phoneNumber" name="" id="" maxlength="10" required>
    
    <br>หลักสูตร
    <select v-model="course" name="" id="" required>
      <option> 4 - 5 ปี</option>
      <option> 4 ปีเทียบเข้าเรียน (2ปี) </option>
      <option> ภาคปกติ</option>
      <option> ภาคสมทบ</option>
    </select>
    
    คณะ
    <select v-model="group" name="" id="" required>
      <option> กรุณาเลือก</option>
      <option> คณะวิทยาศาสตร์</option>
      <option> คณะผลิตกรรมการเกษตร</option>
      <option> คณะวิศวกรรมและอุตสาหกรรมเกษตร</option>
      <option> วิทยาลัยบริหารศาสตร์</option>
      <option> คณะบริหารธุรกิจ</option>
      <option> คณะพัฒนาการท่องเที่ยว</option>
      <option> คณะเทคโนโลยีการประมงและทรัพยากรทางน้ำ</option>
      <option> คณะเศรษฐศาสตร์</option>
      <option> คณะศิลปศาสตร์</option>
      <option> วิทยาลัยพลังงานทดแทน</option>
      <option> คณะสารสนเทศและการสื่อสาร</option>
      <option> คณะสถาปัตยกรรมศาสตร์และการออกแบบสิ่งแวดล้อม</option>
      <option> คณะสัตวศาสตร์และเทคโนโลยี</option>
      <option> มหาวิทยาลัยแม่โจ้-แพร่ เฉลิมพระเกียรติ</option>
      <option> มหาวิทยาลัยแม่โจ้-ชุมพร</option>
    </select><br>
    สาขา
    <select v-model="branch" name="" id="" required> 
      <option>กรุณาเลือก</option>
      <option>วิทยาการคอมพิวเตอร์</option>
      <option>เคมี</option>
      <option>คณิตศาสตร์</option>
      <option>เทคโนโลยีชีวภาพ</option>
      <option>วัสดุศาสตร์</option>
      <option>วิทยาศาสตร์และเทคโนโลยี</option>
      <option>สถิติ</option>
      <option>เทคโนโลยีสารสนเทศ</option>
      <option>ฟิสิกส์</option>
      <option>เกษตรศาสตร์</option>
      <option>เทคโนโลยีการอาหาร</option>
      <option>เทคโนโลยีการผลิต</option>
      <option>เทคโนโลยีพอลิเมอร์</option>
      <option>วิศวกรรมเกษตร</option>
      <option>วิศวกรรมอาหาร</option>
      <option>รัฐประศาสนศาสตร์</option>
      <option>รัฐศาสตร์</option>
      <option>การเงิน</option>
      <option>การจัดการ</option>
      <option>การบัญชี</option>
      <option>การตลาด</option>
      <option>ระบบสารสนเทศ</option>
      <option>การท่องเที่ยวและการโรงแรม</option>
      <option>ประมง</option>
      <option>เศรษฐศาสตร์</option>
      <option>นิเทศศาสตร์</option>
      <option>อังกฤษ</option>
      <option>วิศวกรรมพลังงาน</option>
      <option>ดิจิทัล</option>
      <option>ภูมิสถาปัตยกรรม</option>
      <option>วางแผนภาคและเมือง</option>
      <option>สถาปัตยกรรม</option>
      <option>สัตวศาสตร์</option>
    </select>
    <br>
    <br>
    มีความประสงค์จะขอเปลี่ยน
    <br>คํานําหน้าชื่อ 
    <select name="" id="" required>
      <option></option>
      <option>นาย/Mr.</option>
      <option>นางสาว/Miss</option>
      <option>นาง/Mrs.</option>
    </select><br>
    <br>ชื่อ เป็น ภาษาไทย
    <input v-model="newName" name="" id="" required><br> ภาษาอังกฤษ (พิมพ์ใหญ่)<input name="" value="" required><br>
    <br>นานสกุล เป็น ภาษาไทย
    <input v-model="newLastname" name="" id="" required><br> ภาษาอังกฤษ (พิมพ์ใหญ่)<input name="" value="" required><br>
    <br>ทั้งนี้ได้แนบสําเนา
    <br><input type="checkbox" name="" value="" > หนังสือสําคัญการเปลี่ยนชื่อ - สกุล จํานวน 1 ชุด มาพร้อมนี้<br>
    <input type="checkbox" name="" value=""> หนังสือสําคัญการเปลี่ยนแปลงยศ จํานวน 1 ชุด มาพร้อมนี้
    จึงเรียนมาเพื่อโปรดพิจารณาดําเนินการต่อไปด้วย จักขอบคุณยิ่ง
    <br><span>ความเห็นหน.กลุ่มภารกิจทะเบียนเรียน ประมวลผลและรับเข้า</span>
    <p style="">{{ message }}</p>
    <textarea v-model="message" placeholder=""></textarea>
    <br><span>ความเห็นผู้อํานวยการสํานักบริหารและพัฒนาวิชาการ</span>
    <p style="">{{ message }}</p>
    <textarea v-model="message" placeholder=""></textarea>
    <br><span>สําหรับเจ้าหน้าที่ดําเนินการ</span>
    <p style="">{{ message }}</p>
    <textarea v-model="message" placeholder=""></textarea>
    <br>หมายเหตุ<br>1. ใช้สําหรับนักศึกษาที่กําลังศึกษาเท้านั้น<br>
    2. กรอกรายละเอียดในคําร้องเสร็จเรียบร้อยแล้ว ขอคําแนะนําจากเจ้าหน้าที่

    <br><input type="submit" value="ยืนยันผล">
    
  </form>
</template>


<style scoped>

</style>