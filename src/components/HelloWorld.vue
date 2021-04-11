<template>
  <div class="hello">
    <!-- <h1>{{ msg }}</h1> -->
    <h1>เขียน function แสดงค่าทาง console โดย function รับ parameter 2</h1>
    <div id="two-way-binding" class="demo">
      <p>{{ Showmessage }}</p>
      FirstName:
      <input v-model="firstName" v-on:blur="checkMessage(firstName)" />
      <br />
      LastName:
      <input v-model="lastName" v-on:blur="checkMessage(lastName)" />
    </div>

    <h1>ถ้าหากต้องการ copy “array of object”</h1>
    ใช้ Object.assign([], this.myArray);<br />
    <button v-on:click="chooseOne">run</button>
    <p>data ตั้งต้น : {{ myArrayShow }}</p>
    <p>data Clone : {{ myClonedArrayShow }}</p>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      Showmessage: "Hello Shipppop!",
      firstName: "",
      lastName: "",

      myArray: [
        { a: "a", b: "b" },
        { a: "c", b: "d" },
      ],
      myClonedArray: [],
      myArrayShow: "",
      myClonedArrayShow: "",
    };
  },
  methods: {
    checkMessage() {
      if (this.firstName == "Shippop") {
        this.Showmessage = "Best Online Shipping Platform";
        console.log("this.firstName =='Shippop'", this.Showmessage);
      }
      console.log("firstName: ", this.firstName);
      console.log("lastName: ", this.lastName);
    },
    chooseOne() {
      this.myClonedArray = Object.assign([], this.myArray);
      this.myArrayShow = JSON.stringify(this.myArray);
      this.myClonedArrayShow = JSON.stringify(this.myClonedArray);
      console.log("myClonedArray", this.myClonedArray);
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
