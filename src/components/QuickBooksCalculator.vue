<template>
  <div class="quickbooks-calculator">
    <form>
      <div class="left-col">
        <label for="incomeFromSales">Income From Sales </label>
        <input type="text" name="incomeFromSales" id="incomeFromSales" v-model="incomeFromSales" placeholder="£0"/>

        <label for="construction">Construction </label>
        <input type="text" name="construction" id="construction" v-model="construction" placeholder="£0"/>
      </div>

      <div class="middle-col">
        <label for="commissions">Commissions </label>
        <input type="text" name="commissions" id="commissions" v-model="commissions" placeholder="£0"/>

        <label for="otherIncome">Other Income </label>
        <input type="text" name="otherIncome" id="otherIncome" v-model="otherIncome" placeholder="£0">
      </div>

      <div class="right-col">
        <label for="total">Total </label>
        <input type="text" name="total" id="total" v-model="total" placeholder="£0" class="total">
      </div>
    </form>
  </div> 
</template>

<script>
export default {
  name: 'QuickBooksCalculator',
  data () {
    return {
      incomeFromSales: 0,
      construction: 0,
      commissions: 0,
      otherIncome: 0

    }
  },
  computed: {
    total () {
      let sum = parseInt(this.incomeFromSales) + parseInt(this.construction) + parseInt(this.commissions) + parseInt(this.otherIncome);
      if (isNaN(sum)) {
        sum = 0
      } 
      return sum
    }
  }

}
</script>

<style scoped>

.quickbooks-calculator {
  display: flex;
  justify-content: space-between;
  margin: 40px 0;
}

.quickbooks-calculator form {
  display: flex;
  justify-content: space-between;
  gap: 20px;
}

.quickbooks-calculator input {
  width: 190px;
  margin-bottom: 20px;
}

.quickbooks-calculator input::before {
  content: '£'
}

label {
  display: block;
  margin-bottom: 0px;
  font-size: 12px;
}

.left-col label, .middle-col label {
  font-weight: 200;
}


.right-col {
  font-weight: bold;
}

.left-col input {
  height: 30px;
}

.right-col input {
  border: none;
  height: 98px;
  color: #fff;
  font-size: 60px;
  text-align: center;
  font-weight: 600;
}

.total {
  background: rgb(38,185,71);
  background: linear-gradient(90deg, rgba(38,185,71,1) 0%, rgba(0,191,163,1) 100%);
}

.total ::placeholder { 
  color: #fff;
}
</style>