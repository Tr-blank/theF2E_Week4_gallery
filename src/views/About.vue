<template>
  <main class="about">
    <router-link class="goback" to="/about">CCCLOTHES</router-link>
    <div class="topPic">
      <div class="pic"></div>
      <span>VINTAGE</span>
      <span>DENIM</span>
      <span>TOP</span>
      <span>90</span>
    </div>
    <article>
      <span class="pageName">PRODUCT DETAILS</span>
      <h1>VINTAGE DENIM</h1> 
      <h2>Kogi Cosby sweater ethical squid irony </h2>
      <p>In the tumultuous business of cutting-in and attending to a whale, there is much running backwards and forwards among the crew. Now hands are wanted here, and then again hands are wanted there. There is no staying in any one place; for at one and the same time everything has to be done everywhere. It is much the same with him who endeavors the description of the scene. 

We must now retrace our way a little. It was mentioned that upon first breaking ground in the whale's back, the blubber-hook was inserted into the original hole there cut by the spades of the mates. But how did so clumsy and weighty a mass as that same hook get fixed in that hole? It was inserted there by my particular friend Queequeg, whose duty it was, as harpooneer.</p>
    </article>
  </main>
</template>
<style lang="stylus">
@import '../stylus/normalize'
@import '../stylus/basic'
main
  x-inner()
  text-align left

.topPic
  margin: 128px 12.5%;
  padding: 20%;
  position relative
  .pic
    background-image: url(/img/parker-whitson-571425-unsplash.jpg);
    background-size: cover;
    background-position: center center;
    position absolute
    top 0
    left 0
    width  100%
    height 100%
    z-index 10
  &::before
    content: '';
    background-color: #50e3c2;
    top: -4rem;
    width: 35%;
    height: 50%;
    left: -4rem;
    position: absolute;
    z-index 0
  &::after
    content: '';
    border: 20px solid #50e3c2;
    bottom: -4rem;
    width: 60%;
    height: 44%;
    right: -4rem;
    position: absolute;
    z-index: 0;
  span
    &:nth-child(2)
      position: absolute;
      top: -3rem;
      font-size: 3rem;
      right: 0;
    &:nth-child(3)
      position: absolute;
      top: 0;
      font-size: 3rem;
      left: 100%;
      transform: rotate(90deg);
      transform-origin: top left;
      margin-left: 3rem;
    &:nth-child(4)
      position: absolute;
      bottom: 0;
      font-size: 3rem;
      left: -12.5%;
      transform: rotate(180deg);
      transform-origin: bottom right;
    &:last-child
      position: absolute;
      bottom: 0;
      font-size: 3rem;
      left: -12.5%;
      transform: rotate(90deg);
      transform-origin: bottom right;
      margin-left: -1rem;
.goback
  background-color #000
  color #fff
  font-size 1.25rem
  margin-left 12.5%
  padding 2px 5px
  display inline-block

article
  padding 0 12.5% 0 25% 
  position relative
.pageName
  position: absolute;
  top: 0;
  font-size 2.25rem
  left: 12.5%;
  transform: rotate(90deg);
  transform-origin: top left;
  margin-left: 2.25rem;
h1
  font-size 3rem
h2
  font-size 2.25rem
</style>