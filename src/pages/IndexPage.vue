<template>
  <div class="htmlClass">
    <h1>{{ head }}</h1>
    <form>
      <input type="text" id="firstName" v-model="firstName" />
      <input type="text" id="secondName" v-model="secondName" />
      <button @click="submitForm()" class="submitForm">Submit</button>
    </form>
    <h2>{{ first_Name }}</h2>
    <form>
      <input type="text" id="first_Name" v-model="first_Name" />
    </form>
    <h3>{{ LastName }}</h3>
    <form>
      <input type="text" id="LastName" v-model="LastName" />
    </form>
    <h4>{{ Studentid }}</h4>
    <form>
      <input type="text" id="Studentid" v-model="Studentid" />
    </form>
    <h5>{{ NickName }}</h5>
    <form>
      <input type="text" id="Nickname" v-model="NickName" />
    </form>
  </div>
</template>

<script>
export default {
  name: "InputPage",
  data() {
    return {
      head: "วิวัฒนาการของโลกในสมัยใหม่",
      firstName: "",
      secondName: "",

      first_Name: 'เมธาวี',
      LastName: 'จันสม',
      Studentid:'6604101372',
      NickName:'เมย์',
    };
  },
  methods: {
    submitForm() {
      this.$emit("submit form");
    },
  },
};
</script>

<style scoped></style>
