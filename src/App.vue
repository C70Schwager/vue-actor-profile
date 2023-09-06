<script setup>

const theRock = {
    name: 'Dwayne Johnson',
    nickName: "The Rock", 
    wellKnownMovie: "Fast and Furious",
    birthYear: 1972,
    imageOneLink: "https://pyxis.nymag.com/v1/imgs/a28/baa/af21c34604358b5af8cee2994a28b9954f-3-Dwayne-Johnson.rsquare.w330.jpg",
    imageTwoLink: "https://esq.h-cdn.co/assets/17/26/768x768/square-1498756423-the-rock.jpg",
    quote: "It's not about the car you drive. It's about the size of the arm hanging out of the window.",
    quoteTwo: "Success isn't always about greatness. It's about consistency. Consistent hard work leads to success. Greatness will come.",
    quoteThree: "Success isn't always about greatness. It's about consistency. Consistent hard work leads to success. Greatness will come."
};

function showFirstQuote() {
   alert(theRock.quote);
}

function showSecondQuote() {
   alert(theRock.quoteTwo);
}

function showThirdQuote() {
   alert(theRock.quoteThree);
}

function getRandomQuote() {
  alert(tomHardy.memorableQuote);
}
function getRandomQuote() {
  alert(tomHardy.adviceQuote);
}

export const tomHardy = {
    fullName: 'Edward Thomas Hardy',
    popularRole: "Bane in The Dark Knight Rises",
    birthPlace: "Hammersmith, London, England",
    awardsWon: ["BAFTA Award for Best Actor in a Supporting Role"],
    notableSeries: "Peaky Blinders",
    startYear: 2001,
    currentYear: new Date().getFullYear(),
    imagePortrait: "https://media.gq.com/photos/5e6128d2398289000862596e/1:1/w_805,h_805,c_limit/tom-hardy-lead-840-social.jpg",
    imageBane: "https://static1.moviewebimages.com/wordpress/wp-content/uploads/2022/08/tom-hardy-bane-the-dark-knight-rises.jpeg",
    memorableQuote: "You mustn't be afraid to dream a little bigger, darling.",
    adviceQuote: "I'm from a nice, suburban, middle-class family, but my tattoos remind me where I've been.",
    funFact: "He has a mix of tattoos, some of which he got for film roles!"
};

</script>

<template>
    <h1>{{theRock.name}} Actor Profile</h1>
        <br>
    <p><strong>Name:  </strong>{{theRock.nickName}}</p>
        <br>
    <p><strong>Well known Movie:  </strong>{{theRock.wellKnownMovie}}</p>
        <br>
    <p><strong>Birth Year:  </strong>{{theRock.birthYear}}</p>
        <br>
    <p><strong>Age:  </strong>{{new Date().getFullYear() - theRock.birthYear}}</p>
        <br>
    <img :src="theRock.imageTwoLink"><br><br>
    <button @click="showFirstQuote">The First Quote</button><br>
    <button @click="showSecondQuote">The Second Quote</button><br>
    <button @click="showThirdQuote">The Third Quote</button>
        <br>

    <h1>{{tomHardy.fullName}} Actor Profile</h1>
        <br>
    <ul>
        <li><strong>Popular Role:  </strong>{{ tomHardy.popularRole }}</li>
          <br>
        <li><strong>Birth Place:  </strong>{{ tomHardy.birthPlace }}</li>
          <br>
        <li><strong>Notable Series:  </strong>{{ tomHardy.notableSeries }}</li>
          <br>
        <li><strong>Starting Year:  </strong>{{ tomHardy.startYear }}</li>
          <br>
        <li><strong>Current Year:  </strong>{{ tomHardy.currentYear }}</li>
          <br>
      <img :src="tomHardy.imagePortrait"><br>
      <img :src="tomHardy.imageBane"><br>
      <button @click="getRandomQuote"></button><br>
      <button @click="adviceQuote">The Adviced Quote</button><br>
      <button @click="adviceQuote">The Adviced Quote</button><br>

        




funFact

    </ul>

    
    

</template>



<style scoped>
  body {
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }
  h1 {
    font-size: 44px;
  }
  p, li {
    font-size: 24px;
    font-weight: 200;
  }
  strong {
    font-weight: 300;
  }

  img {
    margin-top: 10px;
  }

  button {
    margin: 5px;
    background-color: lime;
  }
  

</style>