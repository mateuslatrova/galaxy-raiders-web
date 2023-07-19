<template>

  <h2> So sad you will leave us... </h2>
  <h2> If you change your mind, just click on "Start game". </h2>
  <h2> I will give you 5 seconds. </h2>

</template>

<script setup>
// Wait for 2 seconds (2000 milliseconds)
setTimeout(() => {
  // Code to be executed after the delay
  console.log("Waited for 5 seconds");
  window.location.href = "https://www.google.com";
}, 5000);

</script>