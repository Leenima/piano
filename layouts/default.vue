<template>
  <div>
    <nav class="breadcrumb">
      <ul>
        <li><nuxt-link to="/"><i class="fas fa-home"></i>홈으로</nuxt-link></li>
      </ul>
      <li>
        <nuxt-link to="/names"><i class="fas fa-palette"></i>피아노 색 정하기</nuxt-link>
      </li>
    </nav>
    <Nuxt />
    <footer class="footer">
      <div class="content has-text-centered">
        <i class ="fas fa-copyright"></i> 2020-2021, 모든 저작권은 <strong>피아노의 모든것</strong>에 있습니다.
      </div>
    </footer>
  </div>
</template>
