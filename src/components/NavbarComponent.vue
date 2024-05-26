<template>
  <nav
    class="navbar fixed z-50 w-full font-normal text-white bg-[#00000075] lg:px-10 xl:px-32 flex justify-between items-center"
  >
    <div class="navbar-start flex items-center">
      <a class="btn btn-ghost">
        <img src="/logo.png" alt="VMetA Logo" />
      </a>
    </div>

    <div class="navbar-center hidden lg:flex flex-grow justify-center">
      <ul class="menu menu-horizontal px-1 text-xl font-normal">
        <li><a>Home</a></li>
        <li><a>About</a></li>
        <li><a>Blog</a></li>
        <li><a>Cart</a></li>
      </ul>
    </div>

    <div class="navbar-end flex items-center">
      <div class="dropdown lg:hidden">
        <div tabIndex="0" role="button" class="btn btn-ghost">
          <img src="/menu.svg" class="w-6 h-6" alt="menu" />
        </div>
        <ul
          tabIndex="0"
          className="menu menu-sm dropdown-content -left-[150px] mt-3 z-[1] p-2 shadow bg-base-100 rounded-box w-52"
        >
          <li><a>Home</a></li>
          <li><a>About</a></li>
          <li><a>Blog</a></li>
          <li><a>Cart</a></li>
          <li class="mb-3">
            <a
              class="btn btn-sm flex border-[#52057B] rounded-[16px] bg-transparent font-normal text-white text-xl hover:bg-[#52057B] pb-8"
              >login</a
            >
          </li>
          <li>
            <a
              class="btn btn-sm rounded-[16px] bg-[#52057b85] font-medium text-xl text-white hover:bg-transparent hover:border-[#52057B] pb-8"
              >Sign Up</a
            >
          </li>
        </ul>
      </div>

      <div class="hidden lg:flex gap-[2.4375rem]">
        <a
          class="btn border-[#52057B] rounded-[16px] bg-transparent font-normal text-white text-xl hover:bg-[#52057B]"
          >login</a
        >
        <a
          class="btn rounded-[16px] bg-[#52057b85] font-medium text-xl text-white hover:bg-transparent hover:border-[#52057B]"
          >Sign Up</a
        >
      </div>
    </div>
  </nav>
</template>

<script setup></script>

<style scoped></style>
