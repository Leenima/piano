<template>
  <div>
    <section class="hero is-link">
      <div class="hero-body">
        <p class="title">
          <i class="fas fa-glass-martini-alt" /> 피아노의
          <i class="fas fa-glass-cheers" /> 모든것
        </p>
        <p class="subtitle">
          피아노의 색상을 선택해주세요
        </p>
      </div>
    </section>

    <hr>

    <section class="columns">
      <div class="column">
        <table class="table">
          <thead>
            <tr>
              <th>번호</th>
              <th>색깔</th>
            </tr>
          </thead>
          <tbody>
            <template v-for="pos in tablepianoColor1.length">
              <tr :key="pos">
                <td>{{ pos }}</td>
                <td>{{ tablepianoColor1[pos - 1] }}</td>
              </tr>
            </template>
          </tbody>
        </table>
        <div class="content">
          <span class="tag is-danger">출처</span>
          <a href="https://www.usability.gov/how-to-and-tools/methods/color-basics.html">
            www.usability.gov
          </a>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
import pianoColor1 from '~/assets/colors1.json'
import pianoColor2 from '~/assets/colors2.json'
export default {
  data () {
    return {
      tablepianoColor1: pianoColor1.colors,
      tablepianoColor2: pianoColor2.colors
    }
  }
}
</script>
