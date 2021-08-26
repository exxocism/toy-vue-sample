<template>
  <div class="menu">Vue ti ful man</div>
  <div class="list" v-for="a,i in textman" :key="a">{{a}} <br />
    <div class="semi-text"> {{textman[i]}} </div> <hr /></div>
  <div class="maintext">
      <ul>
        <li>This is a sample message <img src="./assets/logo.png" width="20" alt="vue" @click="suckcount=!suckcount; sucktext = (suckcount)? '굿':'노굿'"/> {{sucktext}}</li>
      </ul>
      <p class="talkbox">
        function ({{testval}});
      </p>
    </div> 
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      textman : ['Yousuck', 'Yousuck2', 'I suck' ],
      textman2 : [ 1, 3, 5 ],
      testval : 'you suck man',
      suckcount : true,
      sucktext : '굿',
    }
  }
}
</script>

<style>
#app {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  /* color: #2c3e50; */
  /* margin-top: 60px; */
}
.menu {
  background : darkslategray;
  padding : 23px;
  color : white;
  /* border-radius : 5px; */
  font-weight: 600;
  font-size: 20px;
  width : 100%;
  margin : -10px -10px 30px -10px;
}

.list
{
  font-weight: 600;
  margin-top : 20px;
  text-align : left;
  padding-left: 20px;
  padding-right: 20px;
}

.semi-text
{
  font-weight: 400;
  color : grey;
  margin-top : 10px;
  margin-left : 10px;
}

.talkbox
{
  color : rgb(45, 51, 100);
  background-color : #ddffff;
  border-left: 6px solid #2196F3;
  margin-left : 50px;
  padding : 15px;  
}

.maintext
{
  margin-top : 30px;
  text-align : left;
  margin-left : 10px;
}
</style>
