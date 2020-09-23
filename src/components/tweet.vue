<template>
  <div id="site">
    <button id="button" @click="toggle">Toggle View</button>
    <hr>
    <div class="userone">
      <p v-html="userOne.name"></p>
      <p v-html="userOne.tweet"></p>
      <p v-html="userOne.date"></p>
    </div>
    <br />
    <hr>
    <div class="usertwo">
      <p v-html="userTwo.name"></p>
      <p v-html="userTwo.tweet"></p>
      <p v-html="userTwo.date"></p>
    </div>
    <br />
    <hr>
    <div class="userthree">
      <p v-html="userThree.name"></p>
      <p v-html="userThree.tweet"></p>
      <p v-html="userThree.date"></p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userOne: {
        name: "John",
        tweet: "My cat is a joy, and I want to die trying. A path towards creepy costumes, so it goes. #gooddisease #randomtweet",
        date: "April 5, 2:12 PM"
      },
      userTwo: {
        name: "Billy",
        tweet: "My ingenuity is a pain, and I want to be famous. Excellent mail order software, in fine print. #petnews #randomtweet",
        date: "November 13, 10:46 PM"
      },
      userThree: {
        name: "Karen",
        tweet: "My car is somewhat extravagant, and I want to see other people. More swell alcohol, I think. #powerwad #randomtweet",
        date: "December 29, 12:10 PM"
      }
    };
    function toggle() {
      if(document.getElementById('button').clicked == true){
        document.getElementById('site').style.display = 'grid'
      }
    }
    
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >
#site {
  display: grid;
  display: inline;
}
.userone {
 border-radius: 15px;
 box-shadow: 3px 3px 3px grey;
 padding: 30px; 
 
}
.usertwo {
 border-radius: 15px;
 box-shadow: 3px 3px 3px grey;
 padding: 30px;  
 
 
}
.userthree {
 border-radius: 15px;
 box-shadow: 3px 3px 3px grey;
 padding: 30px;  
}

</style>
