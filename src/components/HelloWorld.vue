<template>
<form>
  <div class="hello">
    <div class="logo">
      <img src="../assets/logo.jpg" />
    </div>
    <div class="heading">
      <div class="subtitle">Welcome to the</div>
      <h1>Pastelle PH Order Form</h1>
      <p>
        After filling this form out, we will be in contact with you to discuss availability of the items ordered and the final payment. Once confirmed, we will give you the payment details. Please provide accurate contact information.
      </p>
    </div>


    <div class="recipient-details">
      <h3>Recipient Details</h3>
      <div class="recipient">
        <div class="item">
          <label>First Name</label>
          <input type="text" />
        </div>
        <div class="item">
          <label>Surname</label>
          <input type="text" />
        </div>
        <div class="item">
          <label>Address</label>
          <input type="text" />
        </div>
        <div class="item">
          <label>Contact Number</label>
          <input type="text" />
        </div>
      </div>

    </div>

    <div class="products">
      <h3>Products</h3>

      <div class="product">
        Tombow ABT Dual Brush Pen
        <div class="pack">
          <div class="label">Pack of 10</div>
          <div class="price">3423</div>
        </div>
        <div class="singles">
          <div class="color">
            Color 1
          </div>
          <div class="color">
            Color 2
          </div>
          <div class="color">
            Color 3
          </div>
          <div class="color">
            Color 3
          </div>
          <div class="color">
            Color 3
          </div>
        </div>
      </div>

    </div>

    <!-- <div class="price">
      sdfsdf
    </div> -->

    <div class="payment">
      <h3>Schedule</h3>
      <p>We would like to remind you that the cutoff for payment is every <strong>Wednesday 6PM and Saturday 6PM</strong>. This means that if we receive your payment after 6pm, your order will be shipped out on the next cutoff. We ship out orders the next day (Thursday and Sunday). <strong>We do not do rush orders.</strong></p>
      





      Please double check your product orders and information supplied before submitting.


      <p>To enable the submit button, we would like you to enter the two days that serve as our payment cutoffs. Please enter in the following format: "[day] and [day]". Example: "Monday and Tuesday".</p>
      <input type="text" />
      
      
      <div class="button">
        Submit Order
      </div>
    </div>
  </div>
  </form>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.hello {
  display: grid;
  width: 100vw;
  grid-template-columns: 200px auto 200px;
  grid-template-rows: auto;
  grid-template-areas:
    "logo heading heading"
    " . recipient-details . "
    " . products products "
    " . payment . ";
  gap: 20px;

}

.logo {
  grid-area: logo;
  box-sizing: border-box;
}

.heading {
  grid-area: heading;
  margin-top: 30px;
  margin-right: 20px;
}

.recipient-details {
  grid-area: recipient-details;
}

.price {
  grid-area: price;
  background: red;
}


.payment {
  grid-area: payment;
}

.products {
  grid-area: products;
}

.recipient {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 10px;
}

.recipient .item {
  box-sizing: border-box;
}

input {
  padding: 5px;
  border-radius: 5px;
  border: 1px solid #edeee9;
  display: block;
  font-size: 15px;
  width: 100%;
  box-sizing: border-box;
}

label {
  text-transform: uppercase;
  /* letter-spacing: 2px; */
  font-size: 14px;
}

/*#feede6*/
/*e3b4b0*/

img {
  width: 200px;
}

.button {
  background: #f6d6c7;
  /* color: #fcd0c7; */
}

h1 {
  margin: 0px;
  padding: 0px;
  font-weight: normal;
}

h1::first-letter {
  margin-left: -2px;
}

.subtitle {
  text-transform: uppercase;
  letter-spacing: 2px;
  font-size: 12px;
}

h3 {
  text-transform: uppercase;
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
