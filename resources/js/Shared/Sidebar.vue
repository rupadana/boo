<template>
  <aside class="left-sidebar">
    <!-- Sidebar scroll-->
    <div class="scroll-sidebar">
      <!-- Sidebar navigation-->
      <nav class="sidebar-nav">
        <ul id="sidebarnav">
          <li class="nav-devider"></li>
          <li class="nav-small-cap">PERSONAL</li>
          <li>
            <Link
              class="waves-effect waves-dark"
              href="/"
              aria-expanded="false"
            >
              <i class="mdi mdi-gauge"> </i>
              <span class="hide-menu"> Home </span>
            </Link>
          </li>
          <li>
            <a
              class="has-arrow waves-effect waves-dark"
              href="#"
              aria-expanded="false"
              ><i class="mdi mdi-bullseye"></i
              ><span class="hide-menu">Indikator</span></a
            >
            <ul aria-expanded="false" class="collapse">
              <li><a href="/indikator">Indikator HDR</a></li>
              <li><a href="/indikator-group">Kelompok Indikator</a></li>
              <li><a href="/indikator-point">Indikator Poin</a></li>
            </ul>
          </li>

          <li>
            <a class="waves-effect waves-dark" aria-expanded="false">
              <i class="mdi mdi-account"></i
              ><span class="hide-menu">Partisipan</span></a
            >
          </li>

          <li>
            <Link
              class="waves-effect waves-dark"
              aria-expanded="false"
              href="/users"
            >
              <i class="fa fa-user"></i>
              <span class="hide-menu">Users </span>
            </Link>
          </li>

          <li>
            <a class="waves-effect waves-dark" aria-expanded="false">
              <i class="fa fa-flag"></i>
              <span class="hide-menu">Roles </span>
            </a>
          </li>
        </ul>
      </nav>
      <!-- End Sidebar navigation -->
    </div>
    <!-- End Sidebar scroll-->
  </aside>
</template>

<script>
import { Link } from "@inertiajs/inertia-vue";
export default {
  components: {
    Link,
  },
};
</script>

<style>
</style>