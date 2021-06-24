<template>
  <div>
    <nav class="breadcrumb">
      <ul>
        <li>
          <nuxt-link to="/">
            <i class="fas fa-home" />홈으로
          </nuxt-link>
        </li>
      </ul>
      <ul>
        <li>
          <nuxt-link to="/instrument1">
            <i class="fas fa-palette" />악기 정하기1
          </nuxt-link>
        </li>
      </ul>
      <li>
        <nuxt-link to="/instrument2">
          <i class="fas fa-palette" />악기 정하기2
        </nuxt-link>
      </li>
      <ul>
        <li>
          <nuxt-link to="/pulsatile">
            <i class="fas fa-palette" />타악기
          </nuxt-link>
        </li>
      </ul>
      <ul>
        <li>
          <nuxt-link to="/keyboard">
            <i class="fas fa-palette" />피아노
          </nuxt-link>
        </li>
      </ul>
      <li>
        <nuxt-link to="/upright">
          <i class="fas fa-palette" />업라이트 피아노
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/grandpiano">
          <i class="fas fa-palette" />그랜드 피아노
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/synthesizer">
          <i class="fas fa-palette" />신디사이저
        </nuxt-link>
      </li>
      <ul>
        <li>
          <nuxt-link to="/wind">
            <i class="fas fa-palette" />관악기의 유례
          </nuxt-link>
        </li>
      </ul>
      <ul>
        <li>
          <nuxt-link to="/harp">
            <i class="fas fa-palette" />현악기-하프
          </nuxt-link>
        </li>
      </ul>
    </nav>
    <Nuxt />
    <footer class="footer">
      <div class="content has-text-centered">
        <i class="fas fa-copyright" />2020-2021, 모든 저작권은 <strong>악기의 모든것</strong>에 있습니다.
      </div>
    </footer>
  </div>
</template>
