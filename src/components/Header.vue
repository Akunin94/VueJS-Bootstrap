<template>
    <header class="fixed-top">
        <nav class="navbar navbar-expand-xl static-top navbar-dark bg-dark">
            <div class="container">
                <a class="navbar-brand h1 mb-0" href="#">
                    <img height="60" src="../assets/logo.png" alt="" loading="lazy"><span class="d-none d-sm-inline">VueJS</span> + <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" class="d-i-block" viewBox="0 0 612 612" role="img" focusable="false"><title>Bootstrap</title><path fill="currentColor" d="M510 8a94.3 94.3 0 0 1 94 94v408a94.3 94.3 0 0 1-94 94H102a94.3 94.3 0 0 1-94-94V102a94.3 94.3 0 0 1 94-94h408m0-8H102C45.9 0 0 45.9 0 102v408c0 56.1 45.9 102 102 102h408c56.1 0 102-45.9 102-102V102C612 45.9 566.1 0 510 0z"></path><path fill="currentColor" d="M196.77 471.5V154.43h124.15c54.27 0 91 31.64 91 79.1 0 33-24.17 63.72-54.71 69.21v1.76c43.07 5.49 70.75 35.82 70.75 78 0 55.81-40 89-107.45 89zm39.55-180.4h63.28c46.8 0 72.29-18.68 72.29-53 0-31.42-21.53-48.78-60-48.78h-75.57zm78.22 145.46c47.68 0 72.73-19.34 72.73-56s-25.93-55.37-76.46-55.37h-74.49v111.4z"></path></svg> <span class="d-none d-sm-inline">Bootstrap</span>
                </a>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse pl-2" id="navbarNavDropdown">
                    <ul class="navbar-nav nav mr-auto">
                        <li class="nav-item" v-for="nav in navbar" :key="nav.index">
                            <a class="nav-link" href="#" :class="{ active: nav.activeClass, disabled: nav.disabledClass }">{{ nav.title }}</a>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            Dropdown link
                            </a>
                            <div class="dropdown-menu mt-0" aria-labelledby="navbarDropdownMenuLink">
                            <a class="dropdown-item" href="#">Action</a>
                            <a class="dropdown-item" href="#">Another action</a>
                            <a class="dropdown-item" href="#">Something else here</a>
                            </div>
                        </li>
                    </ul>
                    <ul class="navbar-nav nav my-4 d-xl-none mr-auto">
                        <li class="nav-item">
                            <a class="nav-link active" href="https://github.com/twbs">GitHub</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="https://twitter.com/getbootstrap">Twitter</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="/docs/4.5/examples/">Examples</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="/docs/4.5/about/overview/">About</a>
                        </li>
                    </ul>
                    <form class="form-inline my-2 my-lg-0">
                        <input class="form-control mr-1 mr-sm-2 w-auto" type="search" placeholder="Search" aria-label="Search">
                        <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
                    </form>
                </div>
            </div>
        </nav>
    </header>
</template>

<script>
export default {
  data() {
      return {
          navbar: [
              {
                title: "Home",
                link : "/",
                activeClass: true,
                disabledClass: false
              },
              {
                title: "Features",
                link : "/features",
                activeClass: false,
                disabledClass: false
              },
              {
                title: "Pricing",
                link : "/price",
                activeClass: false,
                disabledClass: true
              }
          ]
      }
  }
}
</script>

<style>
ul.nav li.dropdown:hover .dropdown-menu{
    display: block;    
}
.fixed-top + * {
    margin-top: 86px;
}
@media all and ( max-width: var(--breakpoint-xl) ) {
    body {
        opacity: 1;
        background: var(--blue);
    }
}
</style>
