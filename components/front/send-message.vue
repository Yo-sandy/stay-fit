<template>
<div class="container" style="padding: 50px">
    <div class="row">
      <div class="col-md-6">
        <div class="wrapper">
          <input class="input" placeholder="Please Enter Text" type="text" >
          <span class="underline"></span>
        </div>
      </div>
      <div class="col-md-6">

      </div>
    </div>
</div>
</template>

<script>
export default {
  name: "send-message"
}
</script>

<style scoped>
.wrapper {
  background-color: #fff;
  border-radius: 2px;
  box-shadow: 0px 2px 1px 0px #ddd;
  box-sizing: border-box;
  height: 300px;
  left: 50%;
  margin: -150px 0 0 -150px;
  position: absolute;
  top: 50%;
  width: 300px;
}
.input {
  background-color: transparent;
  border: none;
  border-bottom: 1px solid #ccc;
  color: #555;
  box-sizing: border-box;
  font-size: 18px;
  height: 50px;
  left: 50%;
  margin: -25px 0 0 -100px;
  padding: 10px 0px;
  position: relative;
  top: 50%;
  width: 200px;
}
.input:focus {
  outline: none;
}
input::-webkit-input-placeholder {
  color: #aaa;
}
input:focus::-webkit-input-placeholder {
  color: dodgerblue;
}
.input:focus + .underline {
  transform: scale(1);
}
.underline {
  background-color: dodgerblue;
  display: inline-block;
  height: 2px;
  left: 50px;
  margin-top: -4px;
  position: absolute;
  top: 185px;
  -webkit-transform: scale(0, 1);
  transform: scale(0, 1);
  -webkit-transition: all 0.5s linear;
  transition: all 0.5s linear;
  width: 202px;
}

</style>
