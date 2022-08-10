<template>
  <div class="invitation">
    <div class="opacity">
      <div class="title-container">
        <span class="title-flicker">
          Te invito a festejar mis 60!
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.invitation {
    /* background-image: url("https://us.123rf.com/450wm/andyvi/andyvi1904/andyvi190400045/121678578-patr%C3%B3n-sin-fisuras-de-memphis-elementos-geom%C3%A9tricos-memphis-al-estilo-de-los-a%C3%B1os-80-ilustraci%C3%B3n-vec.jpg?ver=6"); */
    /* background-image: url("@/assets/invite_background_v2.jpg"); */
    /* background-image: url("@/assets/invite_background.jpg"); */
    /* background-image: linear-gradient( #B63470, #691BB1); */
    /* background-image: linear-gradient( #B63470, #5A00AD); */
    /* background-color: #230454; */
    /* background-image: url("https://www.dropbox.com/s/2ct0i6kc61vp0bh/wall.jpg?raw=1"); */
    background-repeat: no-repeat;
    height: 100%;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.opacity {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* background-color: rgba(35,4,84,0.5) */
}
.title-container{
  margin: auto;
  width: 50%;
  font-family: "Vibur", cursive;
  text-align: center;
  font-size: 80px;
  font-weight: bold;
}
.title-pink {
  color: #FFE3F1;
  text-shadow:
    0 0 6px rgba(232,194,219,0.98),
    0 0 30px rgba(232,194,219,0.34),
    0 0 12px rgba(235,70,147,0.52),
    0 0 22px rgba(235,70,147,0.92),
    0 0 38px rgba(235,70,147,0.78),
    0 0 60px rgba(235,70,147,0.92);
}
.title-pink-v2 {
  color: #FFD9ED;
  text-shadow:
    0 0 6px rgba(224,202,227,0.98),
    0 0 30px rgba(224,202,227,0.34),
    0 0 12px rgba(242,29,143,0.52),
    0 0 22px rgba(242,29,143,0.92),
    0 0 38px rgba(242,29,143,0.78),
    0 0 60px rgba(242,29,143,0.92);
}
.title-pink-v3 {
  color: #FFC7E1;
  text-shadow:
    0 0 6px rgba(224,202,227,0.98),
    0 0 30px rgba(224,202,227,0.34),
    0 0 12px rgba(242,29,129,0.52),
    0 0 22px rgba(242,29,129,0.92),
    0 0 38px rgba(242,29,129,0.78),
    0 0 60px rgba(242,29,129,0.92);
}
.title-flicker {
  color: #FFD9EB;
  animation: neon .08s ease-in-out infinite alternate;
}
.title-blue {
  color: #c6e2ff;
  text-shadow:
    0 0 2px rgba(202,228,225,0.92),
    0 0 10px rgba(202,228,225,0.34),
    0 0 4px rgba(30,132,242,0.52),
    0 0 7px rgba(30,132,242,0.92),
    0 0 11px rgba(30,132,242,0.78),
    0 0 16px rgba(30,132,242,0.92);
}

@keyframes neon {
  from {
    text-shadow:
    0 0 6px rgba(224,202,227,0.98),
    0 0 30px rgba(224,202,227,0.34),
    0 0 12px rgba(242,29,129,0.52),
    0 0 22px rgba(242,29,129,0.92),
    0 0 38px rgba(242,29,129,0.78),
    0 0 60px rgba(242,29,129,0.92);
  }
  to {
    text-shadow:
    0 0 6px rgba(224,202,227,0.98),
    0 0 30px rgba(224,202,227,0.42),
    0 0 12px rgba(242,29,129,0.58),
    0 0 22px rgba(242,29,129,0.84),
    0 0 38px rgba(242,29,129,0.88),
    0 0 60px rgba(242,29,129,1);
  }
}
</style>
