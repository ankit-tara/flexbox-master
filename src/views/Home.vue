<template>
  <div class="wrapper">
    <div class="sidebar">
      <h2>Flex Parent Properties</h2>
      <div class="flexProperty">
        <p>
          flexDirection: <strong>{{ flexDirection }}</strong>
        </p>
        <div class="formItem">
          <label for="row">
            <span>Row</span>
            <input
              type="radio"
              v-model="flexDirection"
              name="flexDirection"
              value="row"
              id="row"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="row-reverse">
            <span>Row-Reverse</span>
            <input
              type="radio"
              v-model="flexDirection"
              name="flexDirection"
              value="row-reverse"
              id="row-reverse"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="column">
            <span>Column</span>
            <input
              type="radio"
              v-model="flexDirection"
              name="flexDirection"
              value="column"
              id="column"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="column-reverse">
            <span>Column-Reverse</span>
            <input
              type="radio"
              v-model="flexDirection"
              name="flexDirection"
              value="column-reverse"
              id="column-reverse"
            />
          </label>
        </div>
      </div>
      <div class="flexProperty">
        <p>
          flex-wrap: <strong>{{ flexWrap }}</strong>
        </p>
        <div class="formItem">
          <label for="no-wrap">
            <span>no-wrap</span>
            <input
              type="radio"
              v-model="flexWrap"
              name="flexWrap"
              value="no-wrap"
              id="no-wrap"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="wrap">
            <span>wrap</span>
            <input
              type="radio"
              v-model="flexWrap"
              name="flexWrap"
              value="wrap"
              id="wrap"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="wrap-reverse">
            <span>wrap-reverse</span>
            <input
              type="radio"
              v-model="flexWrap"
              name="flexWrap"
              value="wrap-reverse"
              id="wrap-reverse"
            />
          </label>
        </div>
      </div>
      <div class="flexProperty">
        <p>
          justify-content: <strong>{{ justifyContent }}</strong>
        </p>
        <div class="formItem">
          <label for="flex-start">
            <span>flex-start</span>
            <input
              type="radio"
              v-model="justifyContent"
              name="justifyContent"
              value="flex-start"
              id="flex-start"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="flex-end">
            <span>flex-end</span>
            <input
              type="radio"
              v-model="justifyContent"
              name="justifyContent"
              value="flex-end"
              id="flex-end"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="center">
            <span>center</span>
            <input
              type="radio"
              v-model="justifyContent"
              name="justifyContent"
              value="center"
              id="center"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="space-between">
            <span>space-between</span>
            <input
              type="radio"
              v-model="justifyContent"
              name="justifyContent"
              value="space-between"
              id="space-between"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="space-around">
            <span>space-around</span>
            <input
              type="radio"
              v-model="justifyContent"
              name="justifyContent"
              value="space-around"
              id="space-around"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="space-evenly">
            <span>space-evenly</span>
            <input
              type="radio"
              v-model="justifyContent"
              name="justifyContent"
              value="space-evenly"
              id="space-evenly"
            />
          </label>
        </div>
      </div>
      <div class="flexProperty">
        <p>
          align-items: <strong>{{ alignItems }}</strong>
        </p>
        <div class="formItem">
          <label for="stretch">
            <span>stretch</span>
            <input
              type="radio"
              v-model="alignItems"
              name="alignItems"
              value="stretch"
              id="stretch"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="flex-start2">
            <span>flex-start</span>
            <input
              type="radio"
              v-model="alignItems"
              name="alignItems"
              value="flex-start"
              id="flex-start2"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="flex-end2">
            <span>flex-end</span>
            <input
              type="radio"
              v-model="alignItems"
              name="alignItems"
              value="flex-end"
              id="flex-end2"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="center2">
            <span>center</span>
            <input
              type="radio"
              v-model="alignItems"
              name="alignItems"
              value="center"
              id="center2"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="baseline">
            <span>baseline</span>
            <input
              type="radio"
              v-model="alignItems"
              name="alignItems"
              value="baseline"
              id="baseline"
            />
          </label>
        </div>
      </div>
      <div class="flexProperty">
        <p>
          align-content: <strong>{{ alignContent }}</strong>
        </p>
        <div class="formItem">
          <label for="stretch2">
            <span>stretch</span>
            <input
              type="radio"
              v-model="alignContent"
              name="alignContent"
              value="stretch"
              id="stretch2"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="flex-start3">
            <span>flex-start</span>
            <input
              type="radio"
              v-model="alignContent"
              name="alignContent"
              value="flex-start"
              id="flex-start3"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="flex-end3">
            <span>flex-end</span>
            <input
              type="radio"
              v-model="alignContent"
              name="alignContent"
              value="flex-end"
              id="flex-end3"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="center3">
            <span>center</span>
            <input
              type="radio"
              v-model="alignContent"
              name="alignContent"
              value="center"
              id="center3"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="space-between2">
            <span>space-between</span>
            <input
              type="radio"
              v-model="alignContent"
              name="alignContent"
              value="space-between"
              id="space-between2"
            />
          </label>
        </div>
        <div class="formItem">
          <label for="space-around2">
            <span>space-around</span>
            <input
              type="radio"
              v-model="alignContent"
              name="alignContent"
              value="space-around"
              id="space-around2"
            />
          </label>
        </div>
      </div>
    </div>
    <div class="main">
      <div class="header">
        <div class="header-left">
          <p>
            Childeren Width: <strong>{{ childWidth }}%</strong>
          </p>
          <input
            v-model="childWidth"
            type="range"
            min="1"
            max="100"
            value="20"
          />
        </div>
        <!-- <div class="header-left">
          <p>
          Parent Height In PX
          </p>
          <input type="number" name="parentHeight" v-model="parentHeight" id="parentHeight">
        </div> -->
        <button class="addBtn" @click="addChild" v-if="childItems.length < 6">
          Add Child
        </button>
      </div>
      <div class="output">
        <div
          style="display: flex; height: 450px"
          v-bind:style="{
            flexDirection: flexDirection,
            alignItems: alignItems,
            justifyContent: justifyContent,
            flexWrap: flexWrap,
            alignContent: alignContent,
           // height: parentHeight+'px',
          }"
        >
          <div
            v-for="(item, index) of childItems"
            :key="index"
            class="item"
            @contextmenu.prevent="$refs.menus.open($event, { index })"
            v-bind:style="{
              width: childWidth + '%',
              order: item.order,
              flexShrink: item.flexShrink,
              flexGrow: item.flexGrow,
              flexBasis: item.flexBasis,
              alignSelf: item.alignSelf,
            }"
          >
            <img v-if="childItems.length > 1" src="../assets/close.svg" alt="" @click="removeChild(index)" class="remove-item">
            <div class="formItem">
              <span class="ItemText">{{ index + 1 }}</span>
            </div>
          </div>
        </div>
      </div>
      <VueContext ref="menus" :closeOnClick="false" v-slot="{ data }">
        <div v-if="data">
          <ChildEdit
            :flexGrow="childItems[data.index].flexGrow"
            :flexBasis="childItems[data.index].flexBasis"
            :flexShrink="childItems[data.index].flexShrink"
            :alignSelf="childItems[data.index].alignSelf"
            :index="data.index"
            :order="childItems[data.index].order"
            @decOrder="decOrder"
            @incOrder="incOrder"
            @flexGrow="flexGrow"
            @flexShrink="flexShrink"
            @flexBasis="flexBasis"
            @alignSelf="alignSelf"
          />
        </div>
      </VueContext>
      <button class="addBtn" style="margin-top:2rem" id="show-modal" @click="showModal = true">Get Code</button>
      <transition name="modal"  v-if="showModal"> 
        <div class="modal-mask">
          <div class="modal-wrapper">
            <div class="modal-container">
              <div class="modal-body">
                <slot name="body">
<img src="../assets/close.svg" class="closeBtn" id="show-modal" @click="showModal = false" alt="">
<vue-code-highlight language="html">
<pre>
    &lt;div class=&quot;parent&quot;&gt;<template><div v-for="(item,index) in childItems" :key="index">
      &lt;div class=&quot;child{{!isEqual(item, index) ? ' child'+(index+1 ): null }}&quot;&gt;{{index+1}}&lt;/div&gt;</div></template>
    &lt;/div&gt;
</pre>
</vue-code-highlight>
<vue-code-highlight language="css">
<pre>
.parent:{
    display:flex;
    flex-direction: {{flexDirection}},
    align-items: {{alignItems}},
    justify-content: {{justifyContent}},
    flex-wrap: {{flexWrap}},
    align-content: {{alignContent}},
    height: {{parentHeight}}px;
  }
.child:{
    order: 1;
    flex-grow: 0;
    flex-shrink: 1;
    flex-basis: auto;
    align-self:auto;
    width: {{childWidth}}%;
  }
</pre>
 {{jsonToCss(childStyles)}}
</vue-code-highlight>
                </slot>
              </div>
            </div>
          </div>
        </div>
      </transition>
    </div>
  </div>
</template>

<script>
import ChildEdit from "../components/ChildEdit";
import VueContext from "vue-context";
import "vue-context/src/sass/vue-context.scss";
import "vue-code-highlight/themes/prism-tomorrow.css";
import "vue-code-highlight/themes/window.css";
import { component as VueCodeHighlight } from 'vue-code-highlight';

export default {
  name: "Home",
  components: {
    ChildEdit,
    VueContext,
    VueCodeHighlight
  },
  data() {
    return {
      showModal: false,
      childItems: [
        {
          order: 1,
          alignSelf: "auto",
          flexGrow: "0",
          flexShrink: "1",
          flexBasis: "auto",
        },
      ],
      childWidth: "20",
      parentHeight: "450",
      flexDirection: "row",
      justifyContent: "flex-start",
      alignItems: "stretch",
      flexWrap: "no-wrap",
      alignContent: "stretch",
      childItem: {
        order: 1,
        alignSelf: "auto",
        flexGrow: "0",
        flexShrink: "1",
        flexBasis: "auto",
      },
      childStyles: {}
    };
  },
  methods: {
    decOrder(index) {
      this.childItems[index].order--;
    },
    incOrder(index) {
      this.childItems[index].order++;
    },
    flexGrow(val, index) {
      this.childItems[index].flexGrow = val;
    },
    flexShrink(val, index) {
      this.childItems[index].flexShrink = val;
    },
    flexBasis(val, index) {
      this.childItems[index].flexBasis = val;
    },
    alignSelf(val, index) {
      this.childItems[index].alignSelf = val;
    },
    addChild() {
      const newChild = Object.assign({}, this.childItem);
      this.childItems.push(newChild);
    },
    camelToKebab(string){
       return string.replace(/([a-z0-9]|(?=[A-Z]))([A-Z])/g, '$1-$2').toLowerCase();
    },
    difference(obj1, obj2){
      let difference = {}
       Object.keys(obj1).forEach(key => {
        if(obj1[key] !== obj2[key]){
          difference[this.camelToKebab(key)] = obj2[key]
        }
      });
      return difference
    },
    isEqual(obj, index){
      if(JSON.stringify(this.childItem) !== JSON.stringify(obj)){
       let difference = this.difference(this.childItem, obj)
       this.childStyles[`.child${index+1}`] = difference
      }
      else{
        delete this.childStyles[`.child${index+1}`]
      }
      return JSON.stringify(this.childItem) === JSON.stringify(obj); 
    },
    jsonToCss(cssjson){
      var styleStr = "";
      for(var i in cssjson){
          styleStr += i + " {\n"
          for(var j in cssjson[i]){
              styleStr += "\t" + j + ":" + cssjson[i][j] + ";\n"     
          }
          styleStr += "}\n"  
      }
      return styleStr
    },
    removeChild(i){
      this.childItems.splice(i, 1);
    }
  },
};
</script>


<style>
.wrapper {
  display: flex;
  justify-content: space-between;
  min-height: 100vh;
}
.sidebar {
  width: 320px;
  text-align: left;
  box-shadow: 0px 1px 20px 0px rgba(0, 0, 0, 0.1);
  padding: 1.5rem;
  overflow: auto;
  height: 100vh;
}

.sidebar h2 {
  margin-bottom: 1.2rem;
}

.main {
  width: calc(100% - 500px);
  margin: 0 auto;
}
.header {
  margin: 2rem 0;
  display: flex;
  justify-content: space-between;
}
.output {
  border: solid 1px #ffcd38;
  padding: 1em;
}

.output .item {
  position: relative;
}
.output .formItem img {
  position: absolute;
  top: 20px;
  left: 20px;
  cursor: pointer;
}
.item {
  padding: 10px;
  background: #ffcd38;
  border: solid 3px #fff;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}
.remove-item{
  position: absolute;
  top:1rem;
  right: 1rem;
  cursor: pointer;
  width: 20px;
}
.item:nth-child(even){
    background: #0075ff;
  }
.flexProperty {
  text-align: left;
  border: solid 2px #ffcd38;
  margin-bottom: 0.75rem;
}
.flexProperty p {
  display: flex;
  /* justify-content: space-between; */
  background: #ffcd38;
  padding: 0.3rem 1rem;
  font-size: 14px;
}
strong {
  margin-left: 10px;
}
.flexProperty .formItem label {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0.3rem 1rem;
  border-bottom: solid 1px #ccc;
  cursor: pointer;
  font-size: 14px;
}

.flexProperty .formItem label:hover {
  background: #eee;
}

.ItemText {
  font-size: 2rem;
  color: #fff;
}

.addBtn {
  background: #ffcd38;
  color: #fff;
  border: none;
  font-size: 1.2rem;
  padding: 0.4rem 1rem;
  border-radius: 5px;
}
.closeBtn {
    filter: invert(0.7);
    top: -1.5rem;
    right: 0rem;
    width: 15px;
    position: absolute;
    cursor: pointer;
}
.results {
  background: #333;
  text-align: left;
  color: #fff;
  margin: 2rem 0;
}

.modal-mask {
  position: fixed;
  z-index: 9998;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  display: table;
  transition: opacity 0.3s ease;
}

.modal-wrapper {
  display: table-cell;
  vertical-align: middle;
}

.modal-container {
  width: 600px;
  margin: 0px auto;
  padding: 20px 30px;
  background-color: #fff;
  border-radius: 2px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.33);
  transition: all 0.3s ease;
  font-family: Helvetica, Arial, sans-serif;
}

.modal-header h3 {
  margin-top: 0;
  color: #42b983;
}

.modal-body {
  margin: 20px 0;
  position: relative;
}

.modal-default-button {
  float: right;
}

.modal-enter {
  opacity: 0;
}

.modal-leave-active {
  opacity: 0;
}

.modal-enter .modal-container,
.modal-leave-active .modal-container {
  -webkit-transform: scale(1.1);
  transform: scale(1.1);
}

.modal-body pre{
  max-height: 450px;
  overflow-y: auto;
}

</style>