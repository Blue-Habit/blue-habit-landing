<template>
  <nav
    class="nav flex flex-wrap items-center justify-between p-4 lg:px-16 sm:px-5 bg-primary"
  >
    <div class="flex flex-no-shrink items-center mr-6 py-3">
      <NuxtLink to="/">
        <img src="@/assets/img/Logo.png" alt="Logo" />
      </NuxtLink>
    </div>

    <input class="menu-btn hidden" type="checkbox" id="menu-btn" />
    <label
      class="menu-icon block cursor-pointer md:hidden px-2 py-4 relative select-none"
      for="menu-btn"
    >
      <span class="navicon flex items-center relative"></span>
    </label>

    <ul class="menu flex justify-end list-reset m-0 w-full md:w-auto">
      <li>
        <a href="#about" class="block md:inline-block px-4 py-3 text-white"
          >About us</a
        >
      </li>

      <li>
        <a
          href="#vision"
          class="block md:inline-block px-4 py-3 no-underline text-white"
          >Vision</a
        >
      </li>

      <li>
        <a
          href="#mission"
          class="block md:inline-block px-4 py-3 no-underline text-white"
          >Mission</a
        >
      </li>
      <li>
        <a
          href="#product"
          class="block md:inline-block px-4 py-3 no-underline text-white"
          >Product</a
        >
      </li>
      <li>
        <a
          href="#team"
          class="block md:inline-block px-4 py-3 no-underline text-white"
          >Team</a
        >
      </li>
    </ul>
  </nav>
  <div>
    <slot />
  </div>
</template>

<script setup></script>

<style>
@media (max-width: 767px) {
  .navicon {
    width: 1.125em;
    height: 0.125em;
  }

  .navicon::before,
  .navicon::after {
    display: block;
    position: absolute;
    width: 100%;
    height: 100%;
    transition: all 0.2s ease-out;
    content: "";
    background: #fff;
  }

  .navicon::before {
    top: 5px;
  }

  .navicon::after {
    top: -5px;
  }

  .menu-btn:not(:checked) ~ .menu {
    display: none;
  }

  .menu-btn:checked ~ .menu {
    display: block;
  }

  .menu-btn:checked ~ .menu-icon .navicon {
    background: transparent;
  }

  .menu-btn:checked ~ .menu-icon .navicon::before {
    transform: rotate(-45deg);
  }

  .menu-btn:checked ~ .menu-icon .navicon::after {
    transform: rotate(45deg);
  }

  .menu-btn:checked ~ .menu-icon .navicon::before,
  .menu-btn:checked ~ .menu-icon .navicon::after {
    top: 0;
  }
}
</style>
