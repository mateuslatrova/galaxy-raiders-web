<template>
  <header>
    <nav class="centered-nav">
      <ul class="horizontal-list">
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/start">Start game</NuxtLink></li>
        <li><NuxtLink to="/leaderboard">Leaderboard</NuxtLink></li>
        <li><NuxtLink to="/quit">Quit game</NuxtLink></li>
      </ul>
    </nav>
  </header>
  <NuxtPage />
</template>

<style>
.centered-nav {
  display: flex;
  justify-content: center;
}

.horizontal-list {
  display: flex;
  list-style: none;
  padding: 0;
}

.horizontal-list li {
  margin: 0 10px;
  font-size: 18px
}

* {
  margin: 0;
  padding: 0;
}
</style>
