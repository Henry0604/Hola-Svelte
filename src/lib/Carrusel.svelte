<script>

</script>


<div class="slidershow middle">

    <div class="slides">
      <input type="radio" name="r" id="r1" checked>
      <input type="radio" name="r" id="r2">
      <input type="radio" name="r" id="r3">
      <input type="radio" name="r" id="r4">
      <input type="radio" name="r" id="r5">
      <div class="slide s1">
        <img src="https://assets.penguinrandomhouse.com/series-images/series-XRU-triad.png" alt="">
      </div>
      <div class="slide">
        <img src="https://lahojadoblada.com/wp-content/uploads/2022/11/franky-montaje.png" alt="">
      </div>
      <div class="slide">
        <img src="https://4.bp.blogspot.com/-DChsad7_5Fo/VL7FHAgHtSI/AAAAAAAACmE/eyqsSwkOYDE/s1600/trilojuegos.png" alt="">
      </div>
      <div class="slide">
        <img src="http://4.bp.blogspot.com/-37qwAE8cpgI/VBPHaakvcKI/AAAAAAAAB0c/QO3tUGGCV8c/s1600/MANZE%2BRUNNER%2Btodos.png" alt="">
      </div>
      <div class="slide">
        <img src="https://cdnx.jumpseller.com/mangabreria/image/4996151/resize/700/700?1610050238" alt="">
      </div>
    </div>

    <div class="navigation">
      <label for="r1" class="bar"></label>
      <label for="r2" class="bar"></label>
      <label for="r3" class="bar"></label>
      <label for="r4" class="bar"></label>
      <label for="r5" class="bar"></label>
    </div>
  </div>



<style>
.slidershow{
  width: 700px;
  height: 400px;
  overflow: hidden;
}
.middle{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
}
.navigation{
  position: absolute;
  bottom: 20px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
}
.bar{
  width: 50px;
  height: 10px;
  border: 2px solid #fff;
  margin: 6px;
  cursor: pointer;
  transition: 0.4s;
}
.bar:hover{
  background: #fff;
}

input[name="r"]{
    position: absolute;
    visibility: hidden;
}

.slides{
  width: 500%;
  height: 100%;
  display: flex;
}

.slide{
  width: 20%;
  transition: 0.6s;
}
.slide img{
  width: 100%;
  height: 100%;
}

#r1:checked ~ .s1{
  margin-left: 0;
}
#r2:checked ~ .s1{
  margin-left: -20%;
}
#r3:checked ~ .s1{
  margin-left: -40%;
}
#r4:checked ~ .s1{
  margin-left: -60%;
}
#r5:checked ~ .s1{
  margin-left: -80%;
}


</style>