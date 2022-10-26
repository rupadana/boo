<template>
  <div>
    <Topbar />
    <Sidebar />

    <div class="page-wrapper">
        <slot />
    </div>
    <footer class="footer">© 2017 Admin Press Admin by themedesigner.in</footer>
  </div>
</template>

<script>
import Topbar from "./Topbar.vue";
import Sidebar from "./Sidebar.vue";
export default {
  components: { Topbar, Sidebar },
  mounted() {
    var i = function () {
        (window.innerWidth > 0 ? window.innerWidth : this.screen.width) < 1170 ? ($("body").addClass("mini-sidebar"),
            $(".navbar-brand span").hide(), $(".scroll-sidebar, .slimScrollDiv").css("overflow-x", "visible").parent().css("overflow", "visible"),
            $(".sidebartoggler i").addClass("ti-menu")) : ($("body").removeClass("mini-sidebar"),
                $(".navbar-brand span").show());
        var i = (window.innerHeight > 0 ? window.innerHeight : this.screen.height) - 1;
        (i -= 70) < 1 && (i = 1), i > 70 && $(".page-wrapper").css("min-height", i + "px");
    };
    i();
  }
};
</script>

<style>
</style>