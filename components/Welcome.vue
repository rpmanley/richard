<template>
  <div class="">
    <div class="line-1 code anim-typewriter">
      Hello... welcome to the portfolio website of Richard Manley...
    </div>
    <div><a href="https://www.linkedin.com/in/richard-manley-68402427" target="_blank">Upwork profile</a></div>
  </div>
</template>

<script>
export default {
  name: 'Welcome'
}
</script>

<style lang="css">
.code {
  background: black;
  color: white;
  padding: 20px;
  font-size: 16px;
  font-family:'DM sans', Courier, monospace;
}

.line-1{
    position: relative;
    top: 50%;  
    /* width: 24em; */
    margin: 0 auto;
    border-right: 2px solid rgba(255,255,255,.75);
    text-align: left;
    white-space: nowrap;
    overflow: hidden;
    transform: translateY(-50%);    
}

/* Animation */
.anim-typewriter{
  animation: typewriter 4s steps(44) 1s 1 normal both,
             blinkTextCursor 500ms steps(44) infinite normal;
}
@keyframes typewriter{
  from{width: 0;}
  to{width: 24em;}
}
@keyframes blinkTextCursor{
  from{border-right-color: rgba(255,255,255,.75);}
  to{border-right-color: transparent;}
}
</style>
