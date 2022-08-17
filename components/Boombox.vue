
<template>
  <div class="main-container">
    <div class="boombox-container">
      <div class="blue-neon-box handle" />
      <div class="boombox-box round-edge blue-neon-box">
        <div class="top-boombox">
          <div class="top-left-speaker smallest-speaker circle pink-neon-box" />
          <div class="name-container purple-neon-box round-edge">
            <span class="name">LAURA</span>
          </div>
          <div class="top-right-speaker smallest-speaker circle pink-neon-box" />
        </div>
        <div class="bottom-boombox">
          <!-- left speaker -->
          <div class="left-speaker speaker circle purple-neon-box">
            <div class="small-speaker circle blue-neon-box">
              <div class="smallest-speaker circle pink-neon-box speaker-animation" />
            </div>
          </div>
          <!-- cassette holder -->
          <div class="round-edge pink-neon-box cassette-holder">
            <div class="left-cassette smallest-speaker circle white-neon-box" />
            <div class="right-cassette smallest-speaker circle white-neon-box" />
          </div>
          <!-- right speaker -->
          <div class="right-speaker speaker circle purple-neon-box">
            <div class="small-speaker circle blue-neon-box">
              <div class="smallest-speaker circle pink-neon-box speaker-animation" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.main-container{
    width: 100%;
}

.boombox-container{
    width: 70%;
    margin: auto;
    aspect-ratio : 2 / 1;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.round-edge {
  border-radius: 15px;
}

.circle {
  border-radius: 50%;
}

.handle{
    border-bottom: 0 !important;
    width: 50%;
    height: 15%;
}

.boombox-box{
    width: 100%;
    height: 85%;
}

.top-boombox{
    width: 100%;
    height: 30%;

    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
}

.bottom-boombox{
    width: 100%;
    height: 70%;

    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
}

.speaker{
    width: 25%;
    aspect-ratio : 1 / 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.small-speaker{
    height: 65%;
    aspect-ratio : 1 / 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.smallest-speaker{
    height: 30%;
    aspect-ratio : 1 / 1;
}

.left-speaker{
    margin-left: 5%;
}

.right-speaker{
    margin-right: 5%;
}

.top-left-speaker{
    margin-left: 3%;
}

.top-right-speaker{
    margin-right: 3%;
}

.name-container{
    flex-grow: 2;
    height: 65%;

    margin-left: 5%;
    margin-right: 5%;

    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.name{
    color: var(--light-shades);
    font-family: 'Chillax-Semibold';
    font-size: calc(1.5vw + 1.5vh);
    letter-spacing: 2px;

    text-shadow:
      0 0 3px rgba(214,211,206,0.92),
      0 0 30px rgba(214,211,206,0.34),
      0 0 12px rgba(205,205,207,0.52),
      0 0 22px rgba(205,205,207,0.92),
      0 0 40px rgba(205,205,207,0.78);
}

.cassette-holder{
    width: 25%;
    aspect-ratio: 2/1;

    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
}

.left-cassette {
    margin-left: 20%;
}

.right-cassette {
    margin-right: 20%;
}

.speaker-animation{
  animation: speakers-pump 0.7s infinite;
}

@keyframes speakers-pump {
  from {
    height: 20%;
  }
  to {
    height: 30%;
  }
}

@media only screen and (min-width: 768px) {
  .boombox-container{
    width: 30%;
  }
}

</style>
