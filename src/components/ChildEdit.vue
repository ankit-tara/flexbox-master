<template>
  <div class="childProperties">
  <div class="flexProperty">
    <p>Child<strong>{{index+1}}</strong></p>
    <div class="formItem">
      <label>
        <span>Order</span>
        <div class="orderBtn">
          <button @click="$emit('decOrder', index)">-</button>
          <span>{{order1}}</span>
          <button @click="$emit('incOrder', index)">+</button>
        </div>
      </label>
    </div>
    <div class="formItem">
      <label for="flex-grow">
        <span>flex-grow</span>
        <input type="number" min="0" v-model="flexGrow1" name="flexGrow1" id="flex-grow" @change="$emit('flexGrow', flexGrow1, index)" @keyup="$emit('flexGrow', flexGrow1, index)">
      </label>
    </div>
    <div class="formItem">
      <label for="flex-shrink">
        <span>flex-shrink</span>
        <input type="number" min="0" v-model="flexShrink1" name="flexShrink1" id="flex-shrink" @change="$emit('flexShrink', flexShrink1, index)" @keyup="$emit('flexShrink', flexShrink1, index)">
      </label>
    </div>
    <div class="formItem">
      <label for="flex-basis">
        <span>flex-basis</span>
        <input type="text" v-model="flexBasis1" name="flexBasis1" id="flex-basis" @keyup="$emit('flexBasis', flexBasis1, index)">
      </label>
    </div>
    <div class="formItem">
      <label for="align-self">
        <span>align-self</span>
        <select v-model="alignSelf1" @change="$emit('alignSelf', alignSelf1, index)">
          <option>auto</option>
          <option>flex-start</option>
          <option>flex-end</option>
          <option>center</option>
          <option>baseline</option>
          <option>stretch</option>
        </select>
    </label>
    </div>
  </div>

  </div>
</template>

<script>
export default {
  name: 'ChildEdit',
  props: {
    index: Number,
    order: Number,
    flexGrow:String,
    flexShrink:String,
    flexBasis:String,
    alignSelf:String
  },
  data() {
    return {
        order1: this.order,
        flexGrow1: this.flexGrow,
        flexShrink1: this.flexShrink,
        flexBasis1: this.flexBasis,
        alignSelf1: this.alignSelf,
    }
  },
  watch:{
    order(val){
      this.order1 = val
    },
    flexGrow(val){
      this.flexGrow1 = val
    },
    flexShrink(val){
      this.flexShrink1 = val
    },
    flexGrow(val){
      this.flexGrow1 = val
    },
    flexBasis(val){
      this.flexBasis1 = val
    },
    alignSelf(val){
      this.alignSelf1 = val
    },
  }
}
</script>

<style>
  .childProperties{
    width: 300px;
  }
  .childProperties .flexProperty{
    margin-bottom: 0;
  }
  .orderBtn button{
    width: 24px;
    height: 20px;
  }
  input[type="number"],
  input[type="text"]{
    width: 75px
  }
  .orderBtn span{
    font-size: 1.2rem;
    display: inline-block;
    margin: 0 10px;
  }
  .v-context{
    padding: 0 !important;
  }
</style>
