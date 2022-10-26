<template>
  <header class="topbar">
    <nav class="navbar top-navbar navbar-expand-md navbar-light">
      <!-- ============================================================== -->
      <!-- Logo -->
      <!-- ============================================================== -->
      <div class="navbar-header">
        <a class="navbar-brand" href="/">
          <!-- Logo icon --><b>
            <!--You can put here icon as well // <i class="wi wi-sunset"></i> //-->
            <!-- Dark Logo icon -->
            <img src="/logo.png" alt="homepage" class="dark-logo" width="50" />
            <!-- Light Logo icon -->
            <img src="/logo.png" alt="homepage" class="light-logo" />
          </b>
          <!--End Logo icon -->
          <!-- Logo text --><span>
            <!-- dark Logo text -->
            <!-- <img
              src="/images/text-logo.jpeg"
              alt="homepage"
              class="dark-logo"
              width="120" /> -->
            <!-- Light Logo text -->
            <!-- <img
              src="/images/text-logo.jpeg"
              class="light-logo"
              alt="homepage"
              width="120"
          /> -->
          </span>
        </a>
      </div>
      <!-- ============================================================== -->
      <!-- End Logo -->
      <!-- ============================================================== -->
      <div class="navbar-collapse">
        <!-- ============================================================== -->
        <!-- toggle and nav items -->
        <!-- ============================================================== -->
        <ul class="navbar-nav mr-auto mt-md-0">
          <!-- This is  -->
          <li class="nav-item">
            <a
              class="
                nav-link nav-toggler
                hidden-md-up
                text-muted
                waves-effect waves-dark
              "
              href="javascript:void(0)"
              ><i class="mdi mdi-menu"></i
            ></a>
          </li>
          <li class="nav-item m-l-10">
            <a
              class="
                nav-link
                sidebartoggler
                hidden-sm-down
                text-muted
                waves-effect waves-dark
              "
              href="javascript:void(0)"
              ><i class="ti-menu"></i
            ></a>
          </li>
        </ul>
        <!-- ============================================================== -->
        <!-- User profile and search -->
        <!-- ============================================================== -->
        <ul class="navbar-nav my-lg-0">
          <!-- ============================================================== -->
          <!-- Search -->
          <!-- ============================================================== -->
          <!-- ============================================================== -->
          <!-- Language -->
          <!-- ============================================================== -->
          <!-- ============================================================== -->
          <!-- Profile -->
          <!-- ============================================================== -->

          <li class="nav-item dropdown">
            <a
              class="
                nav-link
                dropdown-toggle
                text-muted
                waves-effect waves-dark
              "
              href=""
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
              <div class="avatar">Rupadana</div>
            </a>
            <div class="dropdown-menu dropdown-menu-right scale-up">
              <ul class="dropdown-user">
                <li>
                  <div class="dw-user-box">
                    <div class="u-img">
                      <div class="avatar">Rupadana</div>
                    </div>
                    <div class="u-text">
                      <h4>Rupadana</h4>
                      <p class="text-muted">admin@gmail.com</p>
                    </div>
                  </div>
                </li>
                <li role="separator" class="divider"></li>
                <li>
                  <a href="#"><i class="fa fa-power-off"></i> Logout</a>
                </li>
              </ul>
            </div>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
export default {};
</script>

<style>
</style>