<template>
  <div>
    <section class="hero is-link">
      <div class="hero-body">
        <p class="title">
          <i class="fas fa-glass-martini-alt" /> 악기의
          <i class="fas fa-glass-cheers" /> 모든것 2
        </p>
        <p class="subtitle">
          악기를 골라주세요
        </p>
      </div>
    </section>

    <hr>
    <section class="columns" />
    <div class="colums" />
    <table class="table">
      <thead>
        <tr>
          <th>번호</th>
          <th>종류</th>
          <th>악기 이름</th>
        </tr>
      </thead>
      <tbody>
        <template v-for="pos in tableinstrument.length">
          <tr :key="pos">
            <td>{{ pos }}</td>
            <td>{{ tableinstrument[pos - 1].family }}</td>
            <td>{{ tableinstrument[pos - 1].instrument }}</td>
          </tr>
        </template>
      </tbody>
    </table>
    <div class="colums" />
  </div>
</template>

<script>
import axios from 'axios'
export default {
  async asyncData () {
    const instrumentt = await axios.get('https://raw.githubusercontent.com/mobyvb/midi-converter/master/lib/instruments.json')
    return {
      tableinstrument: instrumentt.data,
      tableinstrumentkey: Object.keys(instrumentt.data[0]
      )
    }
  }
}
</script>
