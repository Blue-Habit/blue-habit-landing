<template>
  <nav
    class="nav flex flex-wrap items-center justify-between p-4 px-12 bg-primary"
  >
    <div class="flex flex-no-shrink items-center mr-6 py-3 text-grey-darkest">
      <NuxtLink to="/">
        <img src="@/assets/img/Logo.png" alt="Logo" />
      </NuxtLink>
    </div>

    <input class="menu-btn hidden" type="checkbox" id="menu-btn" />
    <label
      class="menu-icon block cursor-pointer md:hidden px-2 py-4 relative select-none"
      for="menu-btn"
    >
      <span class="navicon bg-grey-darkest flex items-center relative"></span>
    </label>

    <ul
      class="menu border-b md:border-none flex justify-end list-reset m-0 w-full md:w-auto"
    >
      <li class="border-t md:border-none">
        <a href="#about" class="block md:inline-block px-4 py-3 text-white"
          >About us</a
        >
      </li>
      <li class="border-t md:border-none">
        <a
          href="#vision"
          class="block md:inline-block px-4 py-3 no-underline text-white"
          >Vision</a
        >
      </li>
      <li class="border-t md:border-none">
        <a
          href="#mission"
          class="block md:inline-block px-4 py-3 no-underline text-white"
          >Mission</a
        >
      </li>
      <li class="border-t md:border-none">
        <a
          href="#product"
          class="block md:inline-block px-4 py-3 no-underline text-white"
          >Product</a
        >
      </li>
      <li class="border-t md:border-none">
        <a
          href="#team"
          class="block md:inline-block px-4 py-3 no-underline text-white"
          >Team</a
        >
      </li>
    </ul>
  </nav>

  <div class="mx-auto">
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
    background: #3d4852;
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
