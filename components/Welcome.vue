<template>
  <div class="welcome">
    <div class="line typewriter-line-1">
      yarn install richardmanley.com
    </div>
    <div class="line typewriter-line-2">
      loading...
    </div>
    <div class="line typewriter-line-3">
      Front end developer Vue JS, CSS HTML
    </div>
  </div>
</template>

<script>
export default {
  name: 'Welcome'
}
</script>

<style lang="css">
.welcome {
  @apply w-full relative;
}

.line {
  border-right: 2px solid transparent;
  text-align: left;
  white-space: nowrap;
  overflow: hidden;
  font-size: 16px;
  font-family:'DM sans', Courier, monospace;
  padding-bottom: 5px;
}

/* Animation */
.typewriter-line-1{
  animation: typewriter 1.5s steps(34) 1s 1 normal both,
             blinkTextCursor 500ms steps(34) 4 normal;
}
.typewriter-line-2{
  animation: typewriter2 0.7s steps(34) 2s 1 normal both,
             blinkTextCursor2 500ms steps(34) 7 normal;
  animation-delay: 3s;
}
.typewriter-line-3{
  animation: typewriter3 0.7s steps(34) 3s 1 normal both,
             blinkTextCursor2 500ms steps(34) infinite normal;
  animation-delay: 5s;
}
@keyframes typewriter{
  0% {
    width: 0;
  }
  100% {
    width: 19em;
  }
}

@keyframes typewriter2{
  0% {
    width: 0;
  }
  60% {
    with: 0;
  }
  100% {
    width: 6em;
  }
}
@keyframes typewriter3{
  0% {
    width: 0;
  }
  100% {
    width: 22em;
  }
}
@keyframes blinkTextCursor{
  0%  {border-right-color: transparent; }
  50% {border-right-color: rgba(255,255,255,.75);}
  100%  {border-right-color: transparent; }
}

@keyframes blinkTextCursor2{
  0%  {border-right-color: transparent; }
  50%  {border-right-color: transparent; }
  75% {border-right-color: rgba(255,255,255,.75);}
  100%  {border-right-color: transparent; }
}
</style>
