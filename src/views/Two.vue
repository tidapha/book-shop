<template>
  <div class="two">
    <h1>ข้อ 2 - Database Design</h1>
    Normalization = การทํา Normalize จะช่วยแยก Attribute ที่ซํ้าซ้อนกัน ออกไป
    <br />

    การที่มีข้อมูลเดียวกันอยู่ในหลายตาราง ทำให้เกิด การซ้ำของข้อมูล
    ใช้เนื้อที่จัดเก็บข้อมูลมาก หรืออาจเกิดข้อผิดพลาดในการ Update ข้อมูลได้<br />
    การทํา Normalization. เพื่อลดเนื้อที่ในการจัดเก็บข้อมูล และ
    เพื่อลดปัญหาที่ข้อมูลไม่ถูกต้อง(Inconsistency)
  </div>
</template>

<script>
export default {
  name: "Three",
  props: {
    msg: String,
  },
  data() {
    return {
      Showmessage: "Database Design",
    };
  },
  methods: {},
};
</script>
