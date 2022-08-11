<template>
  <div id="container" class="blue-neon">
    <div id="line" />
    <div id="leftSpeaker" />
    <div id="rightSpeaker" />
    <div id="smallleftspeaker" />
    <div id="smallrightspeaker" />
    <div id="smallestleftspeaker" />

    <div id="smallestrightspeaker" />

    <div id="middlebox" />
    <div id="lineinSmallbox" />
    <div id="dotinBoxright" />
    <div id="dotinBoxleft" />

    <div id="recbox" />
    <div id="recboxtop" />
    <div id="bordderleft" />
    <div id="bordderright" />
    <div id="circletopleft" />
    <div id="circletopright" />
    <div id="smallcircletopleft" />
    <div id="smallcircletopright" />

    <div id="smallestcircletopleft" />
    <div id="smallestcircletopright" />

    <div id="recboxtopest" />

    <div id="line1" />
    <div id="line2" />
    <div id="line3" />
    <div id="line4" />

    <div id="smcircle1" />
    <div id="smcircle2" />

    <div id="bgknobL" />
    <div id="bgcircleL1" />
    <div id="bgcircle2" />
    <div id="bgcircleL3" />
    <div id="bgcircleL4" />
    <div id="bgcircleL5" />

    <div id="sLine1" />
    <div id="sLine2" />
    <div id="sLine3" />
    <div id="sLine4" />
    <div id="bgknobR" />
    <div id="adj1" />
    <div id="adj2" />
    <div id="adj3" />
    <div id="adj4" />

    <div id="adjB1" />
    <div id="adjB2" />
    <div id="adjB3" />
    <div id="adjB4" />

    <div id="blockBS" />
    <div id="blockBB1" />
    <div id="blockBB2" />
    <div id="blockBB3" />
    <div id="blockBB4" />
    <div id="blockBB5" />
    <div id="blockBB6" />
    <div id="blockBB7" />
    <div id="blockBB8" />
    <div id="handle" class="blue-neon" />
  </div>
</template>

<script>
export default {

}
</script>

<style>
.pink-neon {
    border: 6px solid #FFADFE !important;
    border-radius: 25px;
    box-shadow:
        0 0 3px rgba(255,194,254,0.98),
        0 0 30px rgba(255,194,254,0.34),
        0 0 12px rgba(255,10,251,0.52),
        0 0 22px rgba(255,10,251,0.92),
        0 0 38px rgba(255,10,251,0.78),
        0 0 50px rgba(255,10,251,0.92)
    ;

        /* inset 0 0 3px rgba(255,194,254,0.98),
        inset 0 0 30px rgba(255,194,254,0.34),
        inset 0 0 12px rgba(255,10,251,0.52),
        inset 0 0 22px rgba(255,10,251,0.92),
        inset 0 0 38px rgba(255,10,251,0.78), */
        /* inset 0 0 60px blue; */
}
.blue-neon {
    border: 6px solid #87FBFC !important;
    border-radius: 25px;
    box-shadow:
        0 0 3px rgba(255,194,254,0.98),
        0 0 30px rgba(255,194,254,0.34),
        0 0 12px rgba(41,203,245,0.52),
        0 0 22px rgba(41,203,245,0.92),
        0 0 38px rgba(41,203,245,0.78),
        0 0 50px rgba(41,203,245,0.92)
    ;

        /* inset 0 0 3px rgba(255,194,254,0.98),
        inset 0 0 30px rgba(255,194,254,0.34),
        inset 0 0 12px rgba(255,10,251,0.52),
        inset 0 0 22px rgba(255,10,251,0.92),
        inset 0 0 38px rgba(255,10,251,0.78), */
        /* inset 0 0 60px blue; */
}
#container{
border: 2px solid;
width: 450px;
height: 250px;
position: absolute;
top: 70px;
left: 0;
right: 0;
margin-left: auto;
margin-right: auto;
}

#line{
position: absolute;
border-top: 1px solid white;
width: 450px;
top: 55px;
left: 0px;
}
#leftSpeaker{
width: 133px;
height: 133px;
border: 2px solid white;
border-radius: 50%;
left: 20px;
position: absolute;
top: 95px;

}
#smallleftspeaker{
width: 106px;
height: 106px;
border: 1px solid white;
border-radius: 50%;
left: 34px;
position: absolute;
top: 110px;

}

#smallestleftspeaker{
width: 32px;
height: 32px;
border: 1px solid white;
border-radius: 50%;
background-color: white;
top: 145px;
position: absolute;
left: 69px;
animation: bumpL .7s infinite;
-webkit-animation: bumpL .7s infinite;
-moz-animation: bumpL .7s infinite;
-ms-animation: bumpL .7s infinite;

}
@-webkit-keyframes bumpL {
from {width: 32px;}
to {width: 38px;}
from{height: 32px;}
to{height: 38px;}

}
@keyframes bumpL {
from {width: 32px;}
to {width: 38px;}
from{height: 32px;}
to{height: 38px;}

}

#rightSpeaker{
width: 133px;
height: 133px;
border: 2px solid white;
border-radius: 50%;
left: 295px;
position: absolute;
top: 95px;
}
#smallrightspeaker{
width: 106px;
height: 106px;
border: 1px solid white;
border-radius: 50%;
left: 309px;
position: absolute;
top: 110px;
}

#smallestrightspeaker{
width: 32px;
height: 32px;
border: 1px solid white;
border-radius: 50%;
background-color: white;
top: 145px;
position: absolute;
left: 344px;
animation: bumpR .7s infinite;
-webkit-animation: bumpR .7s infinite;
-moz-animation: bumpR .7s infinite;
-ms-animation: bumpR .7s infinite;

}
@-webkit-keyframes bumpR {
from {width: 32px;}
to {width: 38px;}
from{height: 32px;}
to{height: 38px;}

}
@keyframes bumpR {
from {width: 32px;}
to {width: 38px;}
from{height: 32px;}
to{height: 38px;}

}

#middlebox{
width: 90px;
height: 65px;
position: absolute;
border: 3px solid white;
top: 122px;
left: 178px;

}
#lineinSmallbox{
border-top: 2px solid white;
width: 91px;
top: 131px;
left: 180px;
position: absolute;
}
#dotinBoxright{
width: 10px;
height: 10px;
position: absolute;
top: 154px;
left: 202px;
border-radius: 50%;
background-color: white;
}
#dotinBoxleft{
width: 10px;
height: 10px;
position: absolute;
top: 153.5px;
left: 236px;
border-radius: 50%;
background-color: white;
}
#recbox{
width: 90px;
height: 20px;
position: absolute;
border: 1px solid white;
top: 200px;
left: 178px;

}
#recboxtop{
width: 110px;
height: 15px;
position: absolute;
border: 1px solid white;
top: 100px;
left: 167px;
}
/*top part*/
#bordderleft{
height: 55px;
position: absolute;
border-left: 1px solid white;
top: 0px;
left: 60px;
}
#bordderright{
height: 55px;
position: absolute;
border-right: 1px solid white;
top: 0px;
left: 389px;
}
#circletopleft{
width: 47px;
height: 47px;
border: 2px solid white;
border-radius: 50%;
left: 4px;
position: absolute;
top: 2px;
}
#circletopright{
width: 47px;
height: 47px;
border: 2px solid white;
border-radius: 50%;
left: 393px;
position: absolute;
top: 2px;
}
#smallcircletopleft{
width: 35px;
height: 35px;
border: 1px solid white;
border-radius: 50%;
left: 11px;
position: absolute;
top: 9px;
}

#smallcircletopright{
width: 35px;
height: 35px;
border: 1px solid white;
border-radius: 50%;
left: 400px;
position: absolute;
top: 9px;
}
#smallestcircletopleft{
width: 13px;
height: 13px;
background-color: white;
border-radius: 50%;
left: 23px;
position: absolute;
top: 20.5px;
}
#smallestcircletopright{
width: 13px;
height: 13px;
background-color: white;
border-radius: 50%;
left: 412px;
position: absolute;
top: 20.5px;
}
#recboxtopest{
width: 290px;
height: 19px;
position: absolute;
border: 1px solid white;
top: 7px;
left: 77px;
}
#line1{
width: 280px;
position: absolute;
border-top: 1px solid white;
top: 10.5px;
left: 82px;
}
#line2{
width: 280px;
position: absolute;
border-top: 1px solid white;
top: 12.7px;
left: 82px;
}
#line3{
width: 280px;
position: absolute;
border-top: 1px solid white;
top: 14.5px;
left: 82px;
}
#line4{
width: 280px;
position: absolute;
border-top: 1px solid white;
top: 21.2px;
left: 82px;
}
#smcircle2{
width: 6px;
height: 6px;
background-color: white;
border-radius: 50%;
left: 76px;
position: absolute;
top: 29px;
}
#smcircle1{
width: 6px;
height: 6px;
background-color: white;
border-radius: 50%;
left: 76px;
position: absolute;
top: 38px;
}
#bgknobL{
width: 20px;
height: 20px;
background-color: white;
border-radius: 50%;
left: 109px;
position: absolute;
top: 32px;
}
#bgcircleL1{
width: 11px;
height: 11px;
background-color: white;
border-radius: 50%;
left: 137px;
position: absolute;
top: 37px;
}
#bgcircle2{
width: 11px;
height: 11px;
background-color: white;
border-radius: 50%;
left: 154px;
position: absolute;
top: 37px;
}
#bgcircleL3{
width: 11px;
height: 11px;
background-color: white;
border-radius: 50%;
left: 169px;
position: absolute;
top: 37px;
}
#bgcircleL4{
width: 11px;
height: 11px;
background-color: white;
border-radius: 50%;
left: 185px;
position: absolute;
top: 37px;
}
#sLine1{
border-left: 1px solid #B6D98D;
height: 10px;
position: absolute;
top: 34px;
left: 145px;
-webkit-transform: rotate(49deg);
        transform: rotate(49deg);
}
#sLine2{
border-right: 1px solid #B6D98D;
height: 7px;
position: absolute;
top: 39px;
left: 162px;
-webkit-transform: rotate(113deg);
        transform: rotate(113deg);
}
#sLine3{
border-right: 1px solid #B6D98D;
height: 7px;
position: absolute;
top: 37px;
left: 178px;
-webkit-transform: rotate(70deg);
        transform: rotate(70deg);
}
#sLine4{
border-right: 1px solid #B6D98D;
height: 7px;
position: absolute;
top: 39px;
left: 188px;
-webkit-transform: rotate(53deg);
        transform: rotate(53deg)
}
#bgknobR{
width: 20px;
height: 20px;
background-color: white;
border-radius: 50%;
left: 330px;
position: absolute;
top: 32px;
}
#adj1{
width: 5px;
height: 22px;
left: 290px;
border: 1px solid white;
position: absolute;
top: 30px;
}
#adj2{
width: 5px;
height: 22px;
left: 277px;
border: 1px solid white;
position: absolute;
top: 30px
}
#adj3{
width: 5px;
height: 22px;
left: 265px;
border: 1px solid white;
position: absolute;
top: 30px
}
#adj4{
width: 5px;
height: 22px;
left: 253px;
border: 1px solid white;
position: absolute;
top: 30px
}
#adjB1{
width: 5px;
height: 6px;
left: 253px;
border: 1px solid white;
background-color: white;
position: absolute;
top: 42px
}
#adjB2{
width: 5px;
height: 6px;
left: 265px;
border: 1px solid white;
background-color: white;
position: absolute;
top: 32px
}
#adjB3{
width: 5px;
height: 6px;
left: 277px;
border: 1px solid white;
background-color: white;
position: absolute;
top: 38px
}
#adjB4{
width: 5px;
height: 6px;
left: 290px;
border: 1px solid white;
background-color: white;
position: absolute;
top: 44px
}
#blockBS{
width: 16px;
height: 16px;
left: 184px;
border: 1px solid white;
position: absolute;
top: 202px
}
#blockBB1{
width: 4px;
height: 16px;
left: 207px;
border: 1px solid white;
background-color: white;
position: absolute;
top: 202px;
}
#blockBB2{
width: 4px;
height: 16px;
left: 214px;
border: 1px solid white;
background-color: white;
position: absolute;
top: 202px;
}
#blockBB3{
width: 4px;
height: 16px;
left: 221px;
border: 1px solid white;
background-color: white;
position: absolute;
top: 202px;
}
#blockBB4{
width: 4px;
height: 16px;
left: 228px;
border: 1px solid white;
background-color: white;
position: absolute;
top: 202px;
}
#blockBB5{
width: 4px;
height: 16px;
left: 235px;
border: 1px solid white;
background-color: white;
position: absolute;
top: 202px;
}
#blockBB6{
width: 4px;
height: 16px;
left: 242px;
border: 1px solid white;
background-color: white;
position: absolute;
top: 202px;
}
#blockBB7{
width: 4px;
height: 16px;
left: 249px;
border: 1px solid white;
background-color: white;
position: absolute;
top: 202px;
}
#blockBB8{
width: 4px;
height: 16px;
left: 256px;
border: 1px solid white;
background-color: white;
position: absolute;
top: 202px;
}
#handle{
border-right: 8px solid white;
border-left: 8px solid white;
border-top: 10px solid white;
border-bottom: 0 !important;
border-radius: 0 !important;
;
height: 30px;
width: 250px;
top: -40px;
left: 95px;
position: absolute;
}
</style>
