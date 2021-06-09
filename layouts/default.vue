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
      <li>
        <nuxt-link to="/instrument1">
          <i class="fas fa-palette" />악기 정하기1
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/instrument2">
          <i class="fas fa-palette" />악기 정하기2
        </nuxt-link>
      </li>
    </nav>
    <Nuxt />
    <footer class="footer">
      <div class="content has-text-centered">
        <i class="fas fa-copyright" />2020-2021, 모든 저작권은 <strong>악기의 모든것</strong>에 있습니다.
      </div>
    </footer>
  </div>
</template>
