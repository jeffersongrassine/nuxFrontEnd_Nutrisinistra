<template>
  <div id="page-top" class="bg-dark fixed-nav sticky-footer">
    <nav
      id="mainNav"
      class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top"
    >
      <nuxt-link to="/dashboard" class="navbar-brand">Sua Logo</nuxt-link>
      <!-- <a class="navbar-brand" href="/dashboard">Sua Logo</a> -->
      <button
        class="navbar-toggler navbar-toggler-right"
        type="button"
        data-toggle="collapse"
        data-target="#navbarCurso"
        aria-control="navbarCurso"
        aria-expanded="false"
        aria-label="Navegação Toggle"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div id="navbarCurso" class="collapse navbar-collapse">
        <ul id="linksaccordion" class="navbar-nav navbar-sidenav">
          <li class="nav-item" data-toggle="tooltip" data-placement="right">
            <a class="nav-link" href="#">
              <i class="fa fa-fw fa-dashboard"></i>
              <span class="nav-link-text">Dashboard</span>
            </a>
          </li>
          <li class="nav-item" data-toggle="tooltip" data-placement="right">
            <a class="nav-link" href="/dashboard/tabelas">
              <i class="fa fa-fw fa-table"></i>
              <span class="nav-link-text">Tabelas</span>
            </a>
          </li>
          <li class="nav-item" data-toggle="tooltip" data-placement="right">
            <a
              class="nav-link nav-link-collapse collapse"
              href="#linkscomponentes"
              data-toggle="collapse"
              data-parent="#linksaccordion"
            >
              <i class="fa fa-fw fa-wrench"></i>
              <span class="nav-link-text">Componentes</span>
            </a>
            <ul id="linkscomponentes" class="sidenav-second-level collapse">
              <li>
                <a href="login.html">Página Login</a>
              </li>
              <li>
                <a href="recuperar.html">Página Recuperar</a>
              </li>
              <li>
                <a href="registro.html">Página Registro</a>
              </li>
              <li>
                <a
                  href="#link3nivel"
                  class="nav-link-collapse collapse"
                  data-toggle="collapse"
                  >Links 3 Niveis</a
                >
                <ul id="link3nivel" class="sidenav-third-level collapse">
                  <li>
                    <a href="#">Link 1</a>
                  </li>
                  <li>
                    <a href="#">Link 2</a>
                  </li>
                  <li>
                    <a href="#">Link 3</a>
                  </li>
                </ul>
              </li>
            </ul>
          </li>
          <li class="nav-item" data-toggle="tooltip" data-placement="right">
            <a
              class="nav-link nav-link-collapse collapse"
              href="#linkspagina"
              data-toggle="collapse"
              data-parent="#linksaccordion"
            >
              <i class="fa fa-fw fa-file"></i>
              <span class="nav-link-text">Páginas</span>
            </a>
            <ul id="linkspagina" class="sidenav-second-level collapse">
              <li>
                <a href="login.html">Página Login</a>
              </li>
              <li>
                <a href="recuperar.html">Página Recuperar</a>
              </li>
              <li>
                <a href="registro.html">Página Registro</a>
              </li>
            </ul>
          </li>
        </ul>
        <ul class="navbar-nav sidenav-toggler">
          <li class="nav-item">
            <a id="sidenavToggler" class="nav-link text-center">
              <i class="fa fa-fw fa-angle-left"></i>
            </a>
          </li>
        </ul>
        <ul class="navbar-nav ml-auto">
          <li class="nav-item dropdown">
            <a
              id="messagesDropdown"
              class="nav-link dropdown-toggle mr-lg-2"
              href="#"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
              <i class="fa fa-fw fa-envelope"></i>
              <span class="d-lg-none">
                Mensagens
                <span class="badge badge-pill badge-primary">12 novas</span>
              </span>
              <span class="indicator text-primary d-none d-lg-block">
                <i class="fa fa-fw fa-circle"></i>
              </span>
            </a>

            <div class="dropdown-menu" aria-labelledby="messagesDropdown">
              <h6 class="dropdown-header">Novas Mensagens</h6>
              <div class="dropdown-divider"></div>
              <a class="dropdown-item" href="#">
                <strong>José Francisco</strong>
                <span class="small float-right text-muted">14:30</span>
                <div class="dropdown-message small">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                </div>
                <div class="dropdown-divider"></div>
              </a>
              <a class="dropdown-item" href="#">
                <strong>Maria Carolina</strong>
                <span class="small float-right text-muted">14:30</span>
                <div class="dropdown-message small">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                </div>
                <div class="dropdown-divider"></div>
              </a>
              <a class="dropdown-item" href="#">
                <strong>Joice da Silva</strong>
                <span class="small float-right text-muted">14:30</span>
                <div class="dropdown-message small">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                </div>
                <div class="dropdown-divider"></div>
                <a href="#" class="dropdown-item small"> Ver todas Mensagens</a>
              </a>
            </div>
          </li>
          <li class="nav-item dropdown">
            <a
              id="alertsDropdown"
              class="nav-link dropdown-toggle mr-lg-2"
              href="#"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
              <i class="fa fa-fw fa-bell"></i>
              <span class="d-lg-none">
                Alertas
                <span class="badge badge-pill badge-warning">5 novos</span>
              </span>
              <span class="indicator text-warning d-none d-lg-block">
                <i class="fa fa-fw fa-circle"></i>
              </span>
            </a>
            <div class="dropdown-menu" aria-labelledby="alertsDropdown">
              <h6 class="dropdown-header">Novos Alertas</h6>
              <div class="dropdown-divider"></div>
              <a class="dropdown-item" href="#">
                <span class="text-success">
                  <strong>
                    <i class="fa fa-fw fa-long-arrow-up"></i>
                    Atualização de Estado
                  </strong>
                </span>
                <span class="small float-right text-muted">14:30</span>
                <div class="dropdown-message small">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                </div>
                <div class="dropdown-divider"></div>
              </a>
              <a class="dropdown-item" href="#">
                <span class="text-danger">
                  <strong>
                    <i class="fa fa-fw fa-long-arrow-down"></i>
                    Atualização de Estado
                  </strong>
                </span>
                <span class="small float-right text-muted">14:30</span>
                <div class="dropdown-message small">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                </div>
                <div class="dropdown-divider"></div>
              </a>
              <a class="dropdown-item" href="#">
                <span class="text-success">
                  <strong>
                    <i class="fa fa-fw fa-long-arrow-up"></i>
                    Atualização de Estado
                  </strong>
                </span>
                <span class="small float-right text-muted">14:30</span>
                <div class="dropdown-message small">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
                  do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                </div>
                <div class="dropdown-divider"></div>
                <a href="#" class="dropdown-item small"> Ver todos Alertas</a>
              </a>
            </div>
          </li>

          <li class="nav-item">
            <form class="form-inline my-2 my-lg-0 mr-lg-2">
              <div class="input-group">
                <input
                  type="text"
                  class="form-control"
                  placeholder="Pesquisar por..."
                />
                <span class="input-group-btn">
                  <button class="btn btn-primary" type="button">
                    <i class="fa fa-search"></i>
                  </button>
                </span>
              </div>
            </form>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              <i class="fa fa-sign-out">Logout</i>
            </a>
          </li>
        </ul>
      </div>
    </nav>
    <div class="content-wrapper">
      <div class="container-fluid">
        <ol class="breadcrumb">
          <li class="breadcrumb-item">
            <a href="index.html">Home</a>
          </li>
          <li class="breadcrumb-item">Página em Branco</li>
        </ol>
        <div class="row">
          <div class="col-12">
            <h1>Titulo da página</h1>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
              reprehenderit in voluptate velit esse cillum dolore eu fugiat
              nulla pariatur. Excepteur sint occaecat cupidatat non proident,
              sunt in culpa qui officia deserunt mollit anim id est laborum.
            </p>
          </div>
        </div>
      </div>
      <footer class="sticky-footer">
        <div class="container">
          <div class="text-center">
            <small>Copyright Seu Site 2017</small>
          </div>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DashboardPage',

  layout: 'dashboard',

  data() {
    return {
      dismissSecs: 10,
      dismissCountDown: 0,
      showDismissibleAlert: false,
    }
  },

  head() {
    return {
      title: 'Dashboard',
    }
  },

  methods: {
    countDownChanged(dismissCountDown) {
      this.dismissCountDown = dismissCountDown
    },
    showAlert() {
      this.dismissCountDown = this.dismissSecs
    },
  },
}
</script>
