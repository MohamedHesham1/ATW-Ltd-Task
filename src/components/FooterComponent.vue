<template>
  <footer class="text-white p-10">
    <div class="max-w-7xl mx-auto">
      <div class="flex flex-col md:flex-row justify-center lg:gap-[5.1875rem]">
        <div class="mb-6 md:mb-0">
          <h2 class="text-2xl font-bold mb-4">Join our weekly digest!</h2>
          <p class="mb-4">
            Get exclusive promotions & updates straight <br />
            to your inbox.
          </p>
          <form class="flex flex-wrap gap-3 lg:flex-nowrap lg:gap-0">
            <input
              type="email"
              placeholder="Enter your email..."
              class="h-[39px] input input-bordered rounded-full w-full max-w-xs mr-2 text-white placeholder-gray-400 placeholder:text-[#D6D5A8] bg-black"
            />
            <button class="btn btn-sm rounded-full bg-black px-4 text-[15pz] text-white h-[39px]">
              Subscribe
            </button>
          </form>
          <button
            class="btn rounded-[16px] bg-[#52057B] bg-opacity-70 font-normal lg:text-xl text-white hover:bg-transparent hover:border-[#52057B] mt-4"
          >
            Create Free Store
          </button>
        </div>
        <div class="flex flex-col md:flex-row justify-between w-full md:w-auto">
          <div class="mb-6 md:mb-0 md:mr-10">
            <h3 class="text-lg font-semibold mb-7">FEATURES</h3>
            <ul>
              <li class="mb-1"><a href="#" class="link link-hover">Build Store</a></li>
              <li class="mb-1"><a href="#" class="link link-hover">Sell NFT</a></li>
              <li class="mb-1"><a href="#" class="link link-hover">Grow Business</a></li>
            </ul>
          </div>
          <div class="mb-6 md:mb-0 md:mr-10">
            <h3 class="text-lg font-semibold mb-7">SERVICES</h3>
            <ul>
              <li class="mb-1"><a href="#" class="link link-hover">Concierge</a></li>
              <li class="mb-1"><a href="#" class="link link-hover">Customization</a></li>
            </ul>
          </div>
          <div class="mb-6 md:mb-0 md:mr-10">
            <h3 class="text-lg font-semibold mb-7">PRODUCT</h3>
            <ul>
              <li class="mb-1"><a href="#" class="link link-hover">About Us</a></li>
              <li class="mb-1"><a href="#" class="link link-hover">Whitepaper</a></li>
              <li class="mb-1"><a href="#" class="link link-hover">$N1 Token</a></li>
              <li class="mb-1"><a href="#" class="link link-hover">Directory</a></li>
            </ul>
          </div>
          <div>
            <h3 class="text-lg font-semibold mb-7">RESOURCES</h3>
            <ul>
              <li class="mb-1"><a href="#" class="link link-hover">Help Center</a></li>
              <li class="mb-1"><a href="#" class="link link-hover">NFTify Branding</a></li>
              <li class="mb-1"><a href="#" class="link link-hover">Success Stories</a></li>
              <li class="mb-1"><a href="#" class="link link-hover">Video Tutorials</a></li>
              <li class="mb-1"><a href="#" class="link link-hover">Contact Support</a></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="bg-[#816797] w-full h-[2px] mt-10"></div>

      <div class="flex flex-col justify-center pt-6 gap-4">
        <p class="text-xl font-medium text-center lg:ml-[100px]">
          The Leading No-code NFT Marketplace Solution
        </p>

        <div class="flex flex-col gap-4 justify-between items-center lg:flex-row lg:gap-0">
          <div class="text-center mt-4">
            <p>© Copyright NFTify Network. All Rights Reserved.</p>
          </div>

          <div class="flex justify-center space-x-4">
            <a
              href="#"
              class="text-gray-400 border rounded-[16px] md:p-[13px] border-white border-opacity-70 hover:text-white"
              ><i class="fab fa-twitter"></i
            ></a>
            <a
              href="#"
              class="text-gray-400 border rounded-[16px] md:p-[13px] border-white border-opacity-70 hover:text-white"
              ><i class="fab fa-telegram"></i
            ></a>
            <a
              href="#"
              class="text-gray-400 border rounded-[16px] md:p-[13px] border-white border-opacity-70 hover:text-white"
              ><i class="fab fa-facebook"></i
            ></a>
            <a
              href="#"
              class="text-gray-400 border rounded-[16px] md:p-[13px] border-white border-opacity-70 hover:text-white"
              ><i class="fab fa-linkedin"></i
            ></a>
            <a
              href="#"
              class="text-gray-400 border rounded-[16px] md:p-[13px] border-white border-opacity-70 hover:text-white"
              ><i class="fab fa-youtube"></i
            ></a>
            <a
              href="#"
              class="text-gray-400 border rounded-[16px] md:p-[13px] border-white border-opacity-70 hover:text-white"
              ><i class="fab fa-instagram"></i
            ></a>
          </div>

          <div class="text-center text-white">
            <a href="#" class="hover:text-white mr-4">Terms of Service</a>
            <a href="#" class="hover:text-white">Privacy Policy</a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup></script>

<style scoped>
.fab {
  font-size: 1.5rem;
}

footer {
  background: linear-gradient(180deg, #52057b 0%, #000000 100%);
}
ul {
  display: flex;
  flex-direction: column;
  gap: 1.75rem;
}
ul li {
  color: #d6d5a8;
  font-size: 12px;
  font-weight: 300;
}

@media (max-width: 768px) {
  div a {
    border: none;
  }
}
</style>
