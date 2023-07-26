<template>
<link href="https://use.fontawesome.com/releases/v5.15.4/css/all.css" rel="stylesheet" />

<link href='https://fonts.googleapis.com/css?family=Roboto:400,500' rel='stylesheet' type='text/css'> 

<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>

<div id="container">

  <div id="holder">

    <div id="image">
      <div class="img jobs"></div>
      <div class="img zuck"></div>
      <div class="img musk"></div>
    </div>

    <div id="right"></div>

    <div id="text">
      <div id="centerText">
        <p class="quote">
          <i class='fa fa-quote-left' style='font-size:30px;color:blue'></i> CodePen is a social development environment. At its heart, it allows you to write code in the browser, and see the results of it as you build. A useful and liberating online code editor for developers of any skill, and particularly empowering for people learning to code. We focus primarily on front-end languages like HTML, CSS, JavaScript, and preprocessing syntaxes that turn into those things. <i class='fa fa-quote-right' style='font-size:30px;color:blue'></i>
        </p>
        <p class="quote">
          <i class='fa fa-quote-left' style='font-size:30px;color:blue'></i> We say social, because CodePen is a community. Most creations on CodePen are public and open source. They are living things that other people and the community can interact with, from a simple hearting, to leaving a comment, to forking and changing for their own needs. <i class='fa fa-quote-right' style='font-size:30px;color:blue'></i>
        </p>
        <p class="quote">
          <i class='fa fa-quote-left' style='font-size:30px;color:blue'></i> People use CodePen for all sorts of things: prototyping new ideas, reduced test cases for bugs, sending clients things to look at, evaluating potential hires, to finding inspiration. People also use CodePen as a sort of resume and portfolio, showing off their best design and development work. <i class='fa fa-quote-right' style='font-size:30px;color:blue'></i>
        </p>
      </div>

      <nav>
        <a id="leftBtn" class="prev"><i class="fa fa-arrow-left"></i></a>
        <a id="rightBtn" class="next"><i class="fa fa-arrow-right"></i></a>
      </nav>
    </div>
  </div>

  <div id="bg">
    <div class="slide jobs-bg"></div>
    <div class="slide zuck-bg"></div>
    <div class="slide musk-bg"></div>
  </div>

  <div id="nav-cirlces">
    <div class="circle"></div>
    <div class="circle"></div>
    <div class="circle"></div>
  </div>

</div>




</template>


<style>




</style>



<script>

$(window).load(function() {
  $(".circle")
    .first()
    .addClass("active");
  $("#bg .slide")
    .first()
    .addClass("active");
  $("#image .img")
    .first()
    .addClass("active");
  $(".quote")
    .first()
    .addClass("active");

  var animate = setInterval(function() {
    var $this = $(".circle"),
      currentActiveBubble = $("#nav-cirlces").find(".active"),
      position = $("#nav-cirlces")
        .children()
        .index(currentActiveBubble),
      num = $(".circle").length;

    if (position < num - 1) {
      $(".active")
        .removeClass("active")
        .next()
        .addClass("active");
    } else {
      $(".circle")
        .removeClass("active")
        .first()
        .addClass("active");
      $("#bg .slide")
        .removeClass("active")
        .first()
        .addClass("active");
      $("#image .img")
        .removeClass("active")
        .first()
        .addClass("active");
      $(".quote")
        .removeClass("active")
        .first()
        .addClass("active");
    }
    position++;
  }, 4500);

  $(".circle").click(function() {
    clearInterval(animate);

    var $this = $(this),
      $siblings = $this.parent().children(),
      position = $siblings.index($this);

    $(".circle")
      .removeClass("active")
      .eq(position)
      .addClass("active");
    $("#bg .slide")
      .removeClass("active")
      .eq(position)
      .addClass("active");
    $("#image .img")
      .removeClass("active")
      .eq(position)
      .addClass("active");
    $(".quote")
      .removeClass("active")
      .eq(position)
      .addClass("active");
  });

  $("#rightBtn , #leftBtn").click(function() {
    clearInterval(animate);

    var $this = $(this),
      currentActiveBubble = $("#nav-cirlces").find(".active"),
      position = $("#nav-cirlces")
        .children()
        .index(currentActiveBubble),
      num = $(".circle").length;

    if ($this.hasClass("next")) {
      if (position < num - 1) {
        $(".active")
          .removeClass("active")
          .next()
          .addClass("active");
      } else {
        $(".circle")
          .removeClass("active")
          .first()
          .addClass("active");
        $("#bg .slide")
          .removeClass("active")
          .first()
          .addClass("active");
        $("#image .img")
          .removeClass("active")
          .first()
          .addClass("active");
        $(".quote")
          .removeClass("active")
          .first()
          .addClass("active");
      }
    } else {
      if (position === 0) {
        $(".circle")
          .removeClass("active")
          .last()
          .addClass("active");
        $("#bg .slide")
          .removeClass("active")
          .last()
          .addClass("active");
        $("#image .img")
          .removeClass("active")
          .last()
          .addClass("active");
        $(".quote")
          .removeClass("active")
          .last()
          .addClass("active");
      } else {
        $(".active")
          .removeClass("active")
          .prev()
          .addClass("active");
      }
    }
  });
});




</script>