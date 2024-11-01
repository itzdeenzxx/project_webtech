<template>
  <div>
    <!-- <h1>Home</h1> -->
    <!-- <div class="mt-5 mx-3">
      <PageProduct />
    </div> -->

    <div class="main">
      <div class="currentplaying">
        <svg height="50px" width="50px" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg" class="spotify">
          <radialGradient gradientUnits="userSpaceOnUse" gradientTransform="translate(0 -534)" r="43.888" cy="572.064"
            cx="33.34" id="ipdIa4~cOclR8yt_ClW93a">
            <stop stop-color="#f4e9c3" offset="0"></stop>
            <stop stop-color="#f8eecd" offset=".219"></stop>
            <stop stop-color="#fdf4dc" offset=".644"></stop>
            <stop stop-color="#fff6e1" offset="1"></stop>
          </radialGradient>
          <path
            d="M51.03,37.34c0.16,0.98,1.08,1.66,2.08,1.66h5.39c2.63,0,4.75,2.28,4.48,4.96	C62.74,46.3,60.64,48,58.29,48H49c-1.22,0-2.18,1.08-1.97,2.34c0.16,0.98,1.08,1.66,2.08,1.66h8.39c1.24,0,2.37,0.5,3.18,1.32	C61.5,54.13,62,55.26,62,56.5c0,2.49-2.01,4.5-4.5,4.5h-49c-1.52,0-2.9-0.62-3.89-1.61C3.62,58.4,3,57.02,3,55.5	C3,52.46,5.46,50,8.5,50H14c1.22,0,2.18-1.08,1.97-2.34C15.81,46.68,14.89,44,13.89,44H5.5c-2.63,0-4.75-2.28-4.48-4.96	C1.26,36.7,3.36,35,5.71,35H8c1.71,0,3.09-1.43,3-3.16C10.91,30.22,9.45,29,7.83,29H4.5c-2.63,0-4.75-2.28-4.48-4.96	C0.26,21.7,2.37,20,4.71,20H20c0.83,0,1.58-0.34,2.12-0.88C22.66,18.58,23,17.83,23,17c0-1.66-1.34-3-3-3h-1.18	c-0.62-0.09-1.43,0-2.32,0h-9c-1.52,0-2.9-0.62-3.89-1.61S2,10.02,2,8.5C2,5.46,4.46,3,7.5,3h49c3.21,0,5.8,2.79,5.47,6.06	C61.68,11.92,60.11,14,57.24,14H52c-2.76,0-5,2.24-5,5c0,1.38,0.56,2.63,1.46,3.54C49.37,23.44,50.62,24,52,24h6.5	c3.21,0,5.8,2.79,5.47,6.06C63.68,32.92,61.11,35,58.24,35H53C51.78,35,50.82,36.08,51.03,37.34z"
            fill="url(#ipdIa4~cOclR8yt_ClW93a)"></path>
          <linearGradient gradientUnits="userSpaceOnUse" gradientTransform="translate(0 -534)" y2="590.253" y1="530.096"
            x2="32" x1="32" id="ipdIa4~cOclR8yt_ClW93b">
            <stop stop-color="#42d778" offset="0"></stop>
            <stop stop-color="#3dca76" offset=".428"></stop>
            <stop stop-color="#34b171" offset="1"></stop>
          </linearGradient>
          <path
            d="M57,32c0,12.837-9.663,23.404-22.115,24.837C33.942,56.942,32.971,57,32,57	c-1.644,0-3.25-0.163-4.808-0.471C15.683,54.298,7,44.163,7,32C7,18.192,18.192,7,32,7S57,18.192,57,32z"
            fill="url(#ipdIa4~cOclR8yt_ClW93b)"></path>
          <path
            d="M41.683,44.394c-0.365,0-0.731-0.181-1.096-0.365c-3.471-2.009-7.674-3.105-12.24-3.105	c-2.559,0-5.116,0.364-7.491,0.912c-0.365,0-0.914,0.183-1.096,0.183c-0.914,0-1.461-0.732-1.461-1.462	c0-0.913,0.547-1.463,1.279-1.643c2.923-0.732,5.846-1.096,8.951-1.096c5.116,0,9.866,1.276,13.885,3.655	c0.548,0.364,0.914,0.73,0.914,1.642C43.145,43.847,42.414,44.394,41.683,44.394z M44.241,38.181c-0.547,0-0.912-0.18-1.279-0.364	c-3.835-2.375-9.135-3.839-15.163-3.839c-2.924,0-5.664,0.366-7.674,0.916c-0.549,0.18-0.731,0.18-1.096,0.18	c-1.096,0-1.827-0.912-1.827-1.826c0-1.096,0.549-1.645,1.461-2.009c2.74-0.73,5.481-1.279,9.317-1.279	c6.213,0,12.241,1.463,16.991,4.384c0.73,0.364,1.096,1.096,1.096,1.826C46.069,37.269,45.337,38.181,44.241,38.181z M47.165,30.876	c-0.548,0-0.731-0.182-1.279-0.364c-4.385-2.559-10.961-4.021-17.356-4.021c-3.289,0-6.577,0.366-9.5,1.096	c-0.366,0-0.731,0.182-1.279,0.182c-1.279,0.183-2.193-0.912-2.193-2.192c0-1.279,0.731-2.009,1.644-2.192	c3.471-1.096,7.125-1.462,11.327-1.462c6.943,0,14.25,1.462,19.731,4.567c0.73,0.366,1.278,1.096,1.278,2.193	C49.357,29.961,48.442,30.876,47.165,30.876z"
            fill="#fff"></path>
        </svg>
        <p class="heading">Currently Playing</p>
      </div>
      <div class="loader">
        <div class="song">
          <p class="name">Time in a Bottle</p>
          <p class="artist">Jim Corce</p>
        </div>
        <div class="albumcover"></div>
        <div class="loading">
          <div class="load"></div>
          <div class="load"></div>
          <div class="load"></div>
          <div class="load"></div>
        </div>
      </div>
      <div class="loader">
        <div class="song">
          <p class="name">My Way</p>
          <p class="artist">Frank Sinatra</p>
        </div>
        <div class="albumcover"></div>
        <div class="play"></div>
      </div>
      <div class="loader">
        <div class="song">
          <p class="name">Lemon Tree</p>
          <p class="artist">Fools Garden</p>
        </div>
        <div class="albumcover"></div>
        <div class="play"></div>
      </div>
    </div>
    <div class="card">
      <div class="top">
        <div class="pfp">
          <div class="playing">
            <div class="greenline line-1"></div>
            <div class="greenline line-2"></div>
            <div class="greenline line-3"></div>
            <div class="greenline line-4"></div>
            <div class="greenline line-5"></div>
          </div>
        </div>
        <div class="texts">
          <p class="title-1">Soldiers Rage</p>
          <p class="title-2">Tha Mechanic</p>
        </div>
      </div>

      <div class="controls">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" height="20" width="24"
          class="volume_button">
          <path clip-rule="evenodd"
            d="M11.26 3.691A1.2 1.2 0 0 1 12 4.8v14.4a1.199 1.199 0 0 1-2.048.848L5.503 15.6H2.4a1.2 1.2 0 0 1-1.2-1.2V9.6a1.2 1.2 0 0 1 1.2-1.2h3.103l4.449-4.448a1.2 1.2 0 0 1 1.308-.26Zm6.328-.176a1.2 1.2 0 0 1 1.697 0A11.967 11.967 0 0 1 22.8 12a11.966 11.966 0 0 1-3.515 8.485 1.2 1.2 0 0 1-1.697-1.697A9.563 9.563 0 0 0 20.4 12a9.565 9.565 0 0 0-2.812-6.788 1.2 1.2 0 0 1 0-1.697Zm-3.394 3.393a1.2 1.2 0 0 1 1.698 0A7.178 7.178 0 0 1 18 12a7.18 7.18 0 0 1-2.108 5.092 1.2 1.2 0 1 1-1.698-1.698A4.782 4.782 0 0 0 15.6 12a4.78 4.78 0 0 0-1.406-3.394 1.2 1.2 0 0 1 0-1.698Z"
            fill-rule="evenodd"></path>
        </svg>
        <div class="volume">
          <div class="slider">
            <div class="green"></div>
          </div>
          <div class="circle"></div>
        </div>
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" height="24" width="24">
          <path clip-rule="evenodd"
            d="M12 21.6a9.6 9.6 0 1 0 0-19.2 9.6 9.6 0 0 0 0 19.2Zm.848-12.352a1.2 1.2 0 0 0-1.696-1.696l-3.6 3.6a1.2 1.2 0 0 0 0 1.696l3.6 3.6a1.2 1.2 0 0 0 1.696-1.696L11.297 13.2H15.6a1.2 1.2 0 1 0 0-2.4h-4.303l1.551-1.552Z"
            fill-rule="evenodd"></path>
        </svg>
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" height="24" width="24">
          <path clip-rule="evenodd"
            d="M21.6 12a9.6 9.6 0 1 1-19.2 0 9.6 9.6 0 0 1 19.2 0ZM8.4 9.6a1.2 1.2 0 1 1 2.4 0v4.8a1.2 1.2 0 1 1-2.4 0V9.6Zm6-1.2a1.2 1.2 0 0 0-1.2 1.2v4.8a1.2 1.2 0 1 0 2.4 0V9.6a1.2 1.2 0 0 0-1.2-1.2Z"
            fill-rule="evenodd"></path>
        </svg>
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" height="24" width="24">
          <path clip-rule="evenodd"
            d="M12 21.6a9.6 9.6 0 1 0 0-19.2 9.6 9.6 0 0 0 0 19.2Zm4.448-10.448-3.6-3.6a1.2 1.2 0 0 0-1.696 1.696l1.551 1.552H8.4a1.2 1.2 0 1 0 0 2.4h4.303l-1.551 1.552a1.2 1.2 0 1 0 1.696 1.696l3.6-3.6a1.2 1.2 0 0 0 0-1.696Z"
            fill-rule="evenodd"></path>
        </svg>
        <div class="air"></div>
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" stroke-width="2" stroke-linejoin="round"
          stroke-linecap="round" class="heart" stroke="currentColor" fill="none" height="20" width="24">
          <path
            d="M3.343 7.778a4.5 4.5 0 0 1 7.339-1.46L12 7.636l1.318-1.318a4.5 4.5 0 1 1 6.364 6.364L12 20.364l-7.682-7.682a4.501 4.501 0 0 1-.975-4.904Z">
          </path>
        </svg>
      </div>
      <div class="song-time">
        <p class="timetext time_now">1:31</p>
        <div class="time">
          <div class="elapsed"></div>
        </div>
        <p class="timetext time_full">3:46</p>
      </div>
    </div>
  </div>
</template>

<script>
// import PageProduct from './PageProduct.vue';
// export default {
//   name: 'TheHome',
//   components: {
//     PageProduct
//   }
// }
</script>

<style>
/* From Uiverse.io by Praashoo7 */
.main {
  background-color: white;
  padding: 1em;
  padding-bottom: 1.1em;
  border-radius: 15px;
  margin: 1em;
}

.loader {
  display: flex;
  flex-direction: row;
  height: 4em;
  padding-left: 1em;
  padding-right: 1em;
  transform: rotate(180deg);
  justify-content: right;
  border-radius: 10px;
  transition: .4s ease-in-out;
}

.loader:hover {
  cursor: pointer;
  background-color: lightgray;
}

.currentplaying {
  display: flex;
  margin: 1em;
}

.spotify {
  width: 50px;
  height: 50px;
  margin-right: 0.6em;
}

.heading {
  color: black;
  font-size: 1.1em;
  font-weight: bold;
  align-self: center;
}

.loading {
  display: flex;
  margin-top: 1em;
  margin-left: 0.3em;
}

.load {
  width: 2px;
  height: 33px;
  background-color: limegreen;
  animation: 1s move6 infinite;
  border-radius: 5px;
  margin: 0.1em;
}

.load:nth-child(1) {
  animation-delay: 0.2s;
}

.load:nth-child(2) {
  animation-delay: 0.4s;
}

.load:nth-child(3) {
  animation-delay: 0.6s;
}

.play {
  position: relative;
  left: 0.35em;
  height: 1.6em;
  width: 1.6em;
  clip-path: polygon(50% 50%, 100% 50%, 75% 6.6%);
  background-color: black;
  transform: rotate(-90deg);
  align-self: center;
  margin-top: 0.7em;
  justify-self: center;
}

.albumcover {
  position: relative;
  margin-right: 1em;
  height: 40px;
  width: 40px;
  background-color: rgb(233, 232, 232);
  align-self: center;
  border-radius: 5px;
}

.song {
  position: relative;
  transform: rotate(180deg);
  margin-right: 1em;
  color: black;
  align-self: center;
}

.artist {
  font-size: 0.6em;
}

@keyframes move6 {
  0% {
    height: 0.2em;
  }

  25% {
    height: 0.7em;
  }

  50% {
    height: 1.5em;
  }

  100% {
    height: 0.2em;
  }
}

/* From Uiverse.io by bociKond */
/* Spotify music card made by: csozi | Website: www.csozi.hu*/

.card {
  position: relative;
  min-width: 100%;
  min-height: 100%;
  background: white;
  border-radius: 10px;
  padding: .5rem;
  display: flex;
  flex-direction: column;
  gap: .3rem;
  box-shadow: 0 10px 40px -25px rgba(100, 100, 100, .5);
  margin-top: 5%;
}


.top {
  position: relative;
  width: 100%;
  display: flex;
  align-items: center;
  gap: 10px;
  margin-block-end: .5rem;
}

.pfp {
  position: relative;
  height: 40px;
  width: 40px;
  background-color: white;
  border-radius: 5px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.title-1 {
  color: black;
  font-size: 1.25rem;
  font-weight: 900;
}

.title-2 {
  color: black;
  font-size: .75rem;
  opacity: .8;
}

/* new */
.song-time {
  width: 100%;
  margin-inline: auto;
  position: relative;
  display: flex;
  align-items: center;
  gap: .3rem;
}

.time {
  width: 90%;
  background-color: #5e5e5e;
  height: .35rem;
  border-radius: 3px;
}

.elapsed {
  width: 42%;
  background-color: #1db954;
  height: 100%;
  border-radius: 3px;
}

.controls {
  color: black;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  width: 100%;
}

.volume {
  height: 100%;
  width: 48px;
}

.air {
  height: 100%;
  width: 48px;
}

.controls svg {
  cursor: pointer;
  transition: 0.1s;
}

.controls svg:hover {
  color: #1db954;
}

.controls .heart:hover {
  color: pink;
}

.volume {
  opacity: 0;
  position: relative;
  transition: 0.2s;
}

.volume .slider {
  height: 4px;
  background-color: #5e5e5e;
  width: 80%;
  border-radius: 2px;
  margin-left: .3rem;
}

.volume .slider .green {
  background-color: #1db954;
  height: 100%;
  width: 80%;
  border-radius: 3px;
}

.volume .circle {
  background-color: white;
  height: 6px;
  width: 6px;
  border-radius: 3px;
  position: absolute;
  right: 20%;
  top: 50%;
  transform: translateY(-50%);
}

.volume_button:hover~.volume {
  opacity: 1;
}

.timetext {
  color: white;
}

.time_now {
  font-size: .8rem;
  background-color: #00000060;
  padding: .5rem;
  border-radius: .5rem;
  background-blend-mode: multiply;
}

.time_full {
  font-size: .8rem;
  background-color: #00000060;
  padding: .5rem;
  border-radius: .5rem;
  background-blend-mode: multiply;
}

.playing {
  display: flex;
  position: relative;
  justify-content: center;
  gap: 1px;
  width: 30px;
  height: 20px;
}

.greenline {
  background-color: #1db954;
  height: 20px;
  width: 2px;
  position: relative;
  transform-origin: bottom;
}

.line-1 {
  animation: infinite playing 1s ease-in-out;
  animation-delay: 0.2s;
}

.line-2 {
  animation: infinite playing 1s ease-in-out;
  animation-delay: 0.5s;
}

.line-3 {
  animation: infinite playing 1s ease-in-out;
  animation-delay: 0.6s;
}

.line-4 {
  animation: infinite playing 1s ease-in-out;
  animation-delay: 0s;
}

.line-5 {
  animation: infinite playing 1s ease-in-out;
  animation-delay: 0.4s;
}

@keyframes playing {
  0% {
    transform: scaleY(0.1);
  }

  33% {
    transform: scaleY(0.6);
  }

  66% {
    transform: scaleY(0.9);
  }

  100% {
    transform: scaleY(0.1);
  }
}
</style>