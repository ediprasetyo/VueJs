<template>
  <div>

  <div class="card">
    <div class="left">
      
      <b> <i class="arrow leftt"></i> Back to Cart</b>
      <div class="row">
        <div class="column1">
          <div class="header">
            <b>Delivery details</b>
          </div>
        <input type="text" placeholder="Email">
        <input type="text" placeholder="Phone Number">
        <input type="textarea" placeholder="Deliver Address" class="message">
        </div>
        <div class="column2">
          <div class="sendas">
            <input type="checkbox" id="checkbox" v-model="checked" class="greenbox">
            <label>Send as Dropshipper</label>
          </div>
          
          <input type="text" placeholder="Dropshipper Name">
          <input type="text" placeholder="Dropshipper Phone Number">
        
        </div>
        <div class="column3">
          <table>
            <div class="headerk">
              <b>Summary</b>
            </div>
            <p>10 item selected</p>
            <br><br><br><br><br><br><br><br><br>
            <p>Cost of goods</p>
            <p>Dropshipping fee</p>
            <div class="headerb">
              <b>Total</b>
            </div>
            <button class="buttonpayment">Continue to Payment</button>
          </table>
        </div>
      </div>
    </div>

  </div>
  </div>
    
</template>

<script>
export default {
  name: 'Step1',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  width: 70%;
  height: 500px;
  background-color:white;
  align: center;
  margin: 0 auto;
  float: none;
  margin-bottom: 10px;
  padding-top: 20px;
  padding-left: 50px;
  padding-bottom: 20px;
  padding-right: 20px;
}
.left {
  text-align: left;
}
.one-line {
  overflow: hidden; 
  text-overflow: ellipsis;
  white-space: nowrap;
}
.header {
  font-size: 40px;
  color: orange;
  padding-top: 30px;
  padding-bottom: 30px;
}
.sendas {
  padding-bottom: 34px;
}
.headerk {
  font-size: 30px;
  color: orange;
  padding-top: 35px;
}
.headerb {
  font-size: 30px;
  color: orange;
  padding-bottom: 10px;
}
.column1 {
  width: 40%;
  float: left;
}
.column2 {
  width: 35%;
  float: left;
  padding-top: 45px;
}
.column3 {
  width: 25%;
  float: left;
}
input[type=text] {
  width: 95%;
  height: 60px;
  font-size: 16px;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 1px solid gray;
}
input[type=text]:focus {
  border: 2px solid green;
}
.message { padding-top: 5px; }
input[type=textarea] {
  width: 95%;
  height: 100px;
  font-size: 16px;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
}
.arrow {
  border: solid black;
  border-width: 0 3px 3px 0;
  display: inline-block;
  padding: 3px;
}

.rightt {
  transform: rotate(-45deg);
  -webkit-transform: rotate(-45deg);
}

.leftt {
  transform: rotate(135deg);
  -webkit-transform: rotate(135deg);
}
.greenbox {
  width: 20px;
  height: 20px;
}
table {
  border-left: 3px solid #FFF8DC;
  padding-left: 10px;
}
.buttonpayment {
  background-color: orange;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 19px;
}
</style>
