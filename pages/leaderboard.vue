<script>

export default {
  data() {
    let leaderboardData = [
      {
          "start": "2023-05-13 19:34:12", 
          "finalScore": 300, 
          "explosions": 15
      },
      {
          "start": "2023-02-16 20:57:27", 
          "finalScore": 280, 
          "explosions": 12
      },
      {
          "start": "2022-09-12 23:46:24", 
          "finalScore": 260, 
          "explosions": 10
      }
    ]
    return { leaderboard : leaderboardData }
  }
};

</script>

<template>

<h1>Leaderboard</h1>
  
<table class="leaderboard-table">
  <thead>
    <tr>
      <th>Rank</th>
      <th>Start time</th>
      <th>Score</th>
      <th>Asteroids hit</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="(item, index) in leaderboard" :key="index">
      <td>{{ index + 1 }}</td>
      <td>{{ item.start }}</td>
      <td>{{ item.finalScore }}</td>
      <td>{{ item.explosions }}</td>
    </tr>
  </tbody>
</table>

</template>

<style>

.leaderboard-table {
    width: 100%;
    border-collapse: collapse;
    font-family: Arial, sans-serif;
}

.leaderboard-table th {
    background-color: #f2f2f2;
    padding: 8px;
    text-align: left;
    font-weight: bold;
}

.leaderboard-table td {
    padding: 8px;
    border-bottom: 1px solid #ddd;
}

.leaderboard-table tbody tr:nth-child(even) {
    background-color: #f9f9f9;
}

.leaderboard-table tbody tr:hover {
    background-color: #e6e6e6;
}

</style>