<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Waktu Tempuh Perjalanan</title>
</head>
<body>
  <div id="app">
    <h1>Hitung Waktu Tempuh Perjalanan</h1>
    <label for="speed">Kecepatan (km/jam): </label>
    <input type="number" id="speed" v-model="speed" placeholder="Masukkan kecepatan">
    
    <label for="distance">Jarak (km): </label>
    <input type="number" id="distance" v-model="distance" placeholder="Masukkan jarak">

    <button @click="calculateTime">Hitung Waktu Tempuh</button>

    <div v-if="time !== null">
      <p>Waktu tempuh yang dibutuhkan: {{ time }} jam</p>
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/vue@2"></script>
  <script src="app.js"></script>
</body>
</html>
