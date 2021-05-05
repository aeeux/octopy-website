
<template>
    <div class="">

    <header class="header">
        <nav class="navbar">
            <img id="logo" href="#" src="~@/assets/octopy-logo.png">
            <input type="checkbox" id="nav" class="hidden">
            <label for="nav" class="nav-toggle">
                <span></span>
                <span></span>
                <span></span>
            </label>
            <div class="wrapper">
                <ul class="menu">
                    <li class="menu-item"><a href="#">Menu Item</a></li>
                    <li class="menu-item"><a href="#">Menu Item</a></li>
                    <li class="menu-item"><a href="#">Menu Item</a></li>
                </ul>
            </div>
        </nav>
    </header>

    </div>
</template>

<script>

export default {
  name: 'Nav',
}
</script>

<style scoped>

    * {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  list-style: none;
  text-decoration: none;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
}

.hidden {
  display: none;
}

#logo {
  width: 5%;
  height: auto;
}

.header {
  width: 100%;
  height: 20vh;
}
.header .navbar {
  display: flex;
  flex-direction: row;
  flex: 1;
  flex-basis: auto;
  justify-content: space-between;
  align-items: center;
  max-width: 90rem;
  width: 100%;
  padding: 1rem 4rem;
  margin: 0 auto;
  position: fixed;
}
.header .navbar .brand {
  font-family: inherit;
  font-size: 1.75rem;
  font-weight: 700;
  line-height: inherit;
  text-transform: uppercase;
  color: #252a32;
}
.header .navbar .menu {
  display: flex;
  flex-direction: row;
  flex: 1;
  flex-basis: auto;
  justify-content: center;
  align-items: center;
}
.header .navbar .menu-item:not(:first-child) {
  margin-left: 2rem;
}
.header .navbar .menu-item a {
  font-family: inherit;
  font-size: 1rem;
  font-weight: 400;
  line-height: inherit;
  color: var(--lightblue);
  text-transform: uppercase;
}

@media only screen and (max-width: 768px) {
  .header .navbar {
    padding: 1rem 2rem;
    margin: 0 auto;
    position: fixed;
  }
  .header .navbar .wrapper {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    opacity: 0;
    background: #f1f5f8;
    transition: all 0.3s ease;
  }
  .header .navbar .wrapper .menu {
    display: flex;
    flex-direction: column;
    position: absolute;
    top: 50%;
    width: 100%;
    transform: translateY(-50%);
  }
  .header .navbar .wrapper .menu-item {
    padding-bottom: 1rem;
    width: 100%;
  }
  .header .navbar .wrapper .menu-item:nth-child(1) a {
    transition-delay: 0.2s;
  }
  .header .navbar .wrapper .menu-item:nth-child(2) a {
    transition-delay: 0.3s;
  }
  .header .navbar .wrapper .menu-item:nth-child(3) a {
    transition-delay: 0.4s;
  }
  .header .navbar .wrapper .menu-item:nth-child(4) a {
    transition-delay: 0.5s;
  }
  .header .navbar .wrapper .menu-item:not(:first-child) {
    margin-left: 0;
  }
  .header .navbar .wrapper .menu-item a {
    padding: 1rem 2rem;
    opacity: 0;
    color: #252a32;
    line-height: 8rem;
    font-size: 3rem;
    font-weight: 600;
    transform: translateX(-20px);
    transition: all 0.3s ease-in-out;
  }
  .header .navbar .nav-toggle {
    display: block;
    position: fixed;
    right: 1rem;
    top: 1rem;
    width: 2.5rem;
    height: 2.5rem;
    cursor: pointer;
    z-index: 999;
  }
  .header .navbar .nav-toggle span {
    display: block;
    width: 20px;
    height: 2px;
    background: var(--lightblue);
    border-radius: 2px;
    margin-left: 14px;
  }
  .header .navbar .nav-toggle span:nth-child(1) {
    margin-top: 16px;
  }
  .header .navbar .nav-toggle span:nth-child(2) {
    margin-top: 4px;
    opacity: 1;
  }
  .header .navbar .nav-toggle span:nth-child(3) {
    margin-top: 4px;
  }
  .header .navbar #nav:checked + .nav-toggle {
    transform: rotate(45deg);
  }
  .header .navbar #nav:checked + .nav-toggle span {
    background: var(--lightblue);
    transition: transform 0.5s ease;
  }
  .header .navbar #nav:checked + .nav-toggle span:nth-child(1) {
    transform: translateY(6px) rotate(180deg);
  }
  .header .navbar #nav:checked + .nav-toggle span:nth-child(2) {
    opacity: 0;
  }
  .header .navbar #nav:checked + .nav-toggle span:nth-child(3) {
    transform: translateY(-6px) rotate(90deg);
  }
  .header .navbar #nav:checked ~ .wrapper {
    z-index: 99;
    opacity: 1;
  }
  .header .navbar #nav:checked ~ .wrapper .menu-item a {
    opacity: 1;
    transform: translateX(0);
  }
}

</style>
