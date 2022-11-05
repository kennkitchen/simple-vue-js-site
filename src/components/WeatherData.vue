<template>
  <div class="w3-container w3-margin-left w3-margin-right">
    <h2>Weather for {{ weather.name }}</h2>
    <table class="w3-table-all">
      <tr>
        <th>Temperature</th>
        <th>Feels Like</th>
        <th>Barometric Pressure</th>
        <th>Humidity</th>
      </tr>
      <tr>
        <td>{{ weather.main.temp }}</td>
        <td>{{ weather.main.feels_like }}</td>
        <td>{{ weather.main.pressure }}</td>
        <td>{{ weather.main.humidity }}</td>
      </tr>
    </table>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: 'WeatherData',
  data() {
    return {
      weather: {
        name: String,
        main: {
          temp: Number,
          feels_like: Number,
          pressure: Number,
          humidity: Number
        },
        wind: {
          speed: Number
        }
      }
    }
  },
  mounted() {
    axios.get('http://api.openweathermap.org/data/2.5/weather?lat=35.0457219&lon=-85.3094883&appid=' + process.env.VUE_APP_WEATHER_API + '&units=imperial')
        .then(res => {
          this.weather = res.data
          this.loading = false
        })
        .catch(error => {
          console.log(error)
          this.error = true
        })
  }
}
</script>