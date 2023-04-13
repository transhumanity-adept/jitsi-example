<script setup>
import { JitsiMeeting } from "@jitsi/vue-sdk";
</script>

<template>
  <div style="display: flex; justify-content: space-around">
    <JitsiMeeting
        domain="localhost:8443"
        room-name="fromwebroomtestroom"
        width="800px"
        height="800px"
        :userInfo="{ displayName: 'patient', email: 'testemail' }"
    >
    </JitsiMeeting>
    <JitsiMeeting
        domain="localhost:8443"
        room-name="fromwebroomtestroom"
        width="800px"
        height="800px"
        :userInfo="{ displayName: 'doctor', email: 'testemail' }"
    >
    </JitsiMeeting>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
