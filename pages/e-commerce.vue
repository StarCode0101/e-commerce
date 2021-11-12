<template>
  <div>
    <nav>
      <div
        class="navbar items-center pb-0 text-black bg-white lg:pt-4 lg:bottom-1 lg:bg-base-100 container mx-auto"
        style="border-bottom-width: 1px"
      >
        <!--Hamburger  On mobile display and flex-none -->
        <div class="flex-none">
          <button
            @click="openMenu"
            class="btn btn-square btn-ghost hover:bg-white lg:hidden"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              class="inline-block w-6 h-6 stroke-current"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              ></path>
            </svg>
          </button>
        </div>
        <!-- Icon always display flex 1 in mobile flex none in lg -->
        <div class="flex-1 px-2 lg:flex-none">
          <span class="text-2xl font-bold"
            ><svg width="138" height="20" xmlns="http://www.w3.org/2000/svg">
              <path
                d="M8.217 20c4.761 0 7.519-.753 7.519-4.606 0-3.4-3.38-4.172-6.66-4.682l-.56-.085-.279-.041-.35-.053c-2.7-.405-3.18-.788-3.18-1.471 0-.478.49-1.331 2.843-1.331 2.455 0 3.493.647 3.493 1.87v.134h4.281v-.133c0-2.389-1.35-5.238-7.774-5.238-5.952 0-7.201 2.584-7.201 4.752 0 3.097 2.763 4.086 7.223 4.675.21.028.433.054.659.081 1.669.197 3.172.42 3.172 1.585 0 1.01-1.615 1.222-3.298 1.222-2.797 0-3.784-.593-3.784-1.92v-.134H.002L0 14.926v.317c.008.79.118 1.913 1.057 2.862C2.303 19.362 4.712 20 8.217 20Zm13.21 0v-7.49c0-2.104.547-4.423 4.176-4.423 3.915 0 3.778 2.777 3.768 4.042V20h4.18v-7.768c0-2.264-.176-7.766-6.732-7.766-2.778 0-4.192.911-5.195 2.28h-.197V4.467H17.22V20h4.207Zm21.959 0c5.094 0 7.787-2.07 8.217-5.405H47.53c-.386 1.02-1.63 1.72-4.143 1.72-2.721 0-3.962-1.03-4.25-3.106h12.527c.24-2.13-.029-5.417-3.026-7.44v.005c-1.312-.915-3.056-1.465-5.251-1.465-5.24 0-8.336 2.772-8.336 7.845 0 5.17 3.02 7.846 8.336 7.846Zm4.099-9.574h-8.188c.486-1.574 1.764-2.431 4.089-2.431 2.994 0 3.755 1.267 4.099 2.431ZM70.499 20V4.457H66.29V6.74h-.176c-1.053-1.377-2.809-2.283-5.677-2.283-6.433 0-7.225 5.293-7.253 7.635v.137c0 2.092.732 7.771 7.241 7.771 2.914 0 4.684-.818 5.734-2.169h.131V20H70.5Zm-8.854-3.623c-3.996 0-4.447-3.032-4.447-4.148 0-1.21.426-4.148 4.455-4.148 3.631 0 4.374 2.044 4.374 4.148 0 2.35-.742 4.148-4.382 4.148ZM88.826 20l-6.529-9.045 6.588-6.488h-5.827l-6.836 6.756V0h-4.187v19.954h4.187V16.94l3.02-2.976L83.6 20h5.226Zm9.9 0c5.094 0 7.786-2.07 8.217-5.405h-4.074c-.387 1.02-1.63 1.72-4.143 1.72-2.721 0-3.962-1.03-4.25-3.106h12.527c.24-2.13-.029-5.417-3.026-7.44v.005c-1.312-.915-3.057-1.465-5.251-1.465-5.24 0-8.336 2.772-8.336 7.845 0 5.17 3.02 7.846 8.336 7.846Zm4.098-9.574h-8.187c.485-1.574 1.763-2.431 4.089-2.431 2.994 0 3.755 1.267 4.098 2.431ZM112.76 20v-6.97c0-2.103.931-4.542 4.05-4.542 1.33 0 2.393.236 2.785.346l.67-3.976c-.728-.16-1.626-.392-2.757-.392-2.665 0-3.622.794-4.486 2.282h-.262V4.466h-4.21V20h4.21Zm17.221 0c4.761 0 7.519-.753 7.519-4.606 0-3.4-3.38-4.172-6.66-4.682l-.56-.085-.279-.041-.349-.053c-2.701-.405-3.181-.788-3.181-1.471 0-.478.49-1.331 2.843-1.331 2.455 0 3.493.647 3.493 1.87v.134h4.282v-.133c0-2.389-1.35-5.238-7.775-5.238-5.952 0-7.201 2.584-7.201 4.752 0 3.097 2.763 4.086 7.224 4.675.21.028.432.054.658.081 1.669.197 3.172.42 3.172 1.585 0 1.01-1.615 1.222-3.298 1.222-2.796 0-3.784-.593-3.784-1.92v-.134h-4.319l-.001.301v.317c.008.79.117 1.913 1.056 2.862 1.246 1.257 3.655 1.895 7.16 1.895Z"
                fill="#1D2026"
                fill-rule="nonzero"
              /></svg
          ></span>
        </div>
        <!-- Link On mobile hide and display on Large -->
        <div class="flex-1 hidden lg:block">
          <nav-links :is-mobile="isMobile"></nav-links>
        </div>
        <div class="flex-none">
          <div class="dropdown dropdown-end">
            <div tabindex="0" class="indicator">
              <div
                class="indicator-item badge text-white i-primary-bg border-0"
                style="height: 1rem; width: 0.5rem"
                v-if="cartCount > 0"
              >
                {{ cartCount }}
              </div>

              <div class="cursor-pointer">
                <svg width="22" height="20" xmlns="http://www.w3.org/2000/svg">
                  <path
                    d="M20.925 3.641H3.863L3.61.816A.896.896 0 0 0 2.717 0H.897a.896.896 0 1 0 0 1.792h1l1.031 11.483c.073.828.52 1.726 1.291 2.336C2.83 17.385 4.099 20 6.359 20c1.875 0 3.197-1.87 2.554-3.642h4.905c-.642 1.77.677 3.642 2.555 3.642a2.72 2.72 0 0 0 2.717-2.717 2.72 2.72 0 0 0-2.717-2.717H6.365c-.681 0-1.274-.41-1.53-1.009l14.321-.842a.896.896 0 0 0 .817-.677l1.821-7.283a.897.897 0 0 0-.87-1.114ZM6.358 18.208a.926.926 0 0 1 0-1.85.926.926 0 0 1 0 1.85Zm10.015 0a.926.926 0 0 1 0-1.85.926.926 0 0 1 0 1.85Zm2.021-7.243-13.8.81-.57-6.341h15.753l-1.383 5.53Z"
                    fill="#69707D"
                    fill-rule="nonzero"
                  />
                </svg>
              </div>
            </div>

            <div
              tabindex="0"
              class="shadow-lg dropdown-content bg-base-100 rounded-md w-80 -mr-5 lg:-mr-0 mt-5 lg:mt-0 lg:w-72"
              :class="[cartCount <= 0 ? 'h-52' : '']"
            >
              <h2 class="font-bold text-sm border-b-2 border-gray-200 py-4 px-4">Cart</h2>

              <div v-if="cartCount <= 0" class="flex h-2/3 items-center justify-center">
                <h2 class="text-gray-500">Your cart is empty</h2>
              </div>
              <div v-else class="flex flex-col py-5 px-4">
                <div class="flex items-center">
                  <img
                    class="flex-none w-11 h-11 rounded-sm"
                    src="~/assets/images/image-product-1-thumbnail.jpg"
                  />
                  <div class="flex-1">
                    <div class="px-2">
                      <p class="text-md font-thin truncate" style="max-width: 13rem">
                        Autumn Limited Edition...
                      </p>
                      <p class="text-md font-thin">
                        ${{ price }} x {{ cartCount
                        }}<span class="font-bold"> ${{ price * cartCount }}</span>
                      </p>
                    </div>
                  </div>
                  <div class="flex-none">
                    <svg
                      width="14"
                      height="16"
                      xmlns="http://www.w3.org/2000/svg"
                      xmlns:xlink="http://www.w3.org/1999/xlink"
                    >
                      <defs>
                        <path
                          d="M0 2.625V1.75C0 1.334.334 1 .75 1h3.5l.294-.584A.741.741 0 0 1 5.213 0h3.571a.75.75 0 0 1 .672.416L9.75 1h3.5c.416 0 .75.334.75.75v.875a.376.376 0 0 1-.375.375H.375A.376.376 0 0 1 0 2.625Zm13 1.75V14.5a1.5 1.5 0 0 1-1.5 1.5h-9A1.5 1.5 0 0 1 1 14.5V4.375C1 4.169 1.169 4 1.375 4h11.25c.206 0 .375.169.375.375ZM4.5 6.5c0-.275-.225-.5-.5-.5s-.5.225-.5.5v7c0 .275.225.5.5.5s.5-.225.5-.5v-7Zm3 0c0-.275-.225-.5-.5-.5s-.5.225-.5.5v7c0 .275.225.5.5.5s.5-.225.5-.5v-7Zm3 0c0-.275-.225-.5-.5-.5s-.5.225-.5.5v7c0 .275.225.5.5.5s.5-.225.5-.5v-7Z"
                          id="a"
                        />
                      </defs>
                      <use fill="#C3CAD9" fill-rule="nonzero" xlink:href="#a" />
                    </svg>
                  </div>
                </div>
                <button class="btn btn-i-primary w-full my-4">Checkout</button>
              </div>
            </div>
          </div>
        </div>

        <div class="flex-none rounded-full w-8 h-8 ml-4">
          <!--  Cart dropdown -->
          <img
            class="avatar cursor-pointer"
            src="~/assets/images/image-avatar.png"
            alt="avatar"
          />
        </div>
      </div>
    </nav>

    <main>
      <div class="container mx-auto flex flex-wrap lg:mt-14 lg:px-4 mb-52">
        <!-- This will hold slides of swiper -->
        <div class="lg:w-2/5 w-full">
          <div
            class="w-full relative flex bg-no-repeat bg-cover bg-center h-60 lg:h-52 items-center"
            :style="{
              backgroundImage:
                'url(' + require(`~/assets/images/${images[index]}.jpg`) + ')',
            }"
            :class="classObject"
            @click="showModal"
          >
            <!-- Controls -->
            <div class="w-full flex justify-between lg:hidden">
              <button
                class="mx-2 btn btn-circle btn-xs bg-white hover:bg-white border-0"
                @click="index == 0 ? (index = images.length - 1) : index--"
              >
                <svg
                  class="control"
                  xmlns="http://www.w3.org/2000/svg"
                  width="16"
                  height="16"
                  viewBox="0 0 16 16"
                >
                  <path
                    fill-rule="evenodd"
                    d="M11.354 1.646a.5.5 0 0 1 0 .708L5.707 8l5.647 5.646a.5.5 0 0 1-.708.708l-6-6a.5.5 0 0 1 0-.708l6-6a.5.5 0 0 1 .708 0z"
                  />
                </svg>
              </button>
              <button
                class="mx-2 btn btn-circle btn-xs bg-white hover:bg-white border-0"
                @click="index + 1 == images.length ? (index = 0) : index++"
              >
                <svg
                  class="control"
                  xmlns="http://www.w3.org/2000/svg"
                  width="16"
                  height="16"
                  viewBox="0 0 16 16"
                >
                  <path
                    fill-rule="evenodd"
                    d="M4.646 1.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1 0 .708l-6 6a.5.5 0 0 1-.708-.708L10.293 8 4.646 2.354a.5.5 0 0 1 0-.708z"
                  />
                </svg>
              </button>
            </div>
          </div>
          <div
            class="hidden lg:grid grid-cols-4 grid-rows-1 gap-4 mt-3 place-content-evenly"
          >
            <div class="image-list" @click.capture="index = 0">
              <img class="h-auto" src="~/assets/images/image-product-1-thumbnail.jpg" />
            </div>
            <div class="image-list" @click.capture="index = 1">
              <img class="h-auto" src="~/assets/images/image-product-2-thumbnail.jpg" />
            </div>
            <div class="image-list" @click.capture="index = 2">
              <img class="h-auto" src="~/assets/images/image-product-3-thumbnail.jpg" />
            </div>
            <div class="image-list" @click.capture="index = 3">
              <img class="h-auto" src="~/assets/images/image-product-4-thumbnail.jpg" />
            </div>
          </div>
        </div>

        <div class="w-full lg:w-3/5 h-6 bg-blue p-0 lg:p-20">
          <!-- This will hold detials -->
          <div class="block px-4 py-5">
            <p class="i-primary text-xs uppercase py-2">Sneaker company</p>
            <p class="text-lg lg:text-5xl py-2 font-bold">
              Fall Limited Edition Sneakers
            </p>
            <p class="text-md text-gray-500 py-5">
              These low-profile sneakers are your perfect casual wear companion. Featuring
              a durable rubber outer soul, they'll withstand everything the weather can
              offer
            </p>
            <div class="flex lg:block items-center">
              <div class="inline-flex flex-1 items-center py-3">
                <div class="text-lg">$125.00</div>
                <div class="text-xs i-primary bg-pale-primary rounded-sm mx-3 px-1 py-1">
                  50%
                </div>
              </div>
              <div class="flex-0 lg:flex-none line-through text-xs font-thin">
                $250.00
              </div>
            </div>

            <div class="flex flex-wrap lg:flex-nowrap lg:space-x-2">
              <button
                class="flex flex-nowrap w-full btn bg-gray-200 border-0 active:bg-gray-200 hover:bg-gray-200 no-animation lg:w-1/5"
              >
                <div
                  class="flex-0 i-primary font-bold cursor-pointer p-4"
                  @click="cartCount == 0 ? '' : cartCount--"
                >
                  <svg
                    width="12"
                    height="4"
                    xmlns="http://www.w3.org/2000/svg"
                    xmlns:xlink="http://www.w3.org/1999/xlink"
                  >
                    <defs>
                      <path
                        d="M11.357 3.332A.641.641 0 0 0 12 2.69V.643A.641.641 0 0 0 11.357 0H.643A.641.641 0 0 0 0 .643v2.046c0 .357.287.643.643.643h10.714Z"
                        id="a"
                      />
                    </defs>
                    <use fill="#FF7E1B" fill-rule="nonzero" xlink:href="#a" />
                  </svg>
                </div>
                <h3 class="flex-1 font-bold text-black">{{ cartCount }}</h3>
                <div
                  class="flex-0 i-primary font-bold cursor-pointer p-4"
                  @click="cartCount >= 0 ? cartCount++ : ''"
                >
                  <svg
                    width="12"
                    height="12"
                    xmlns="http://www.w3.org/2000/svg"
                    xmlns:xlink="http://www.w3.org/1999/xlink"
                  >
                    <defs>
                      <path
                        d="M12 7.023V4.977a.641.641 0 0 0-.643-.643h-3.69V.643A.641.641 0 0 0 7.022 0H4.977a.641.641 0 0 0-.643.643v3.69H.643A.641.641 0 0 0 0 4.978v2.046c0 .356.287.643.643.643h3.69v3.691c0 .356.288.643.644.643h2.046a.641.641 0 0 0 .643-.643v-3.69h3.691A.641.641 0 0 0 12 7.022Z"
                        id="b"
                      />
                    </defs>
                    <use fill="#FF7E1B" fill-rule="nonzero" xlink:href="#b" />
                  </svg>
                </div>
              </button>
              <button
                class="btn btn-i-primary i-primary-shadow w-full my-2 lg:my-0 lg:w-2/5 normal-case"
              >
                <svg width="22" height="20" xmlns="http://www.w3.org/2000/svg">
                  <path
                    d="M20.925 3.641H3.863L3.61.816A.896.896 0 0 0 2.717 0H.897a.896.896 0 1 0 0 1.792h1l1.031 11.483c.073.828.52 1.726 1.291 2.336C2.83 17.385 4.099 20 6.359 20c1.875 0 3.197-1.87 2.554-3.642h4.905c-.642 1.77.677 3.642 2.555 3.642a2.72 2.72 0 0 0 2.717-2.717 2.72 2.72 0 0 0-2.717-2.717H6.365c-.681 0-1.274-.41-1.53-1.009l14.321-.842a.896.896 0 0 0 .817-.677l1.821-7.283a.897.897 0 0 0-.87-1.114ZM6.358 18.208a.926.926 0 0 1 0-1.85.926.926 0 0 1 0 1.85Zm10.015 0a.926.926 0 0 1 0-1.85.926.926 0 0 1 0 1.85Zm2.021-7.243-13.8.81-.57-6.341h15.753l-1.383 5.53Z"
                    fill="#FFFFFF"
                    fill-rule="nonzero"
                  />
                </svg>
                <span class="ml-2 text-sm">Add to cart</span>
              </button>
            </div>
          </div>
        </div>
      </div>
    </main>
    <!-- modal -->
    <div
      v-if="!isMobile"
      class="modal"
      :class="[modalOpen ? 'modal-open' : 'modal-close']"
    >
      <div class="p-0 bg-transparent shadow-none">
        <div
          class="w-full relative flex bg-no-repeat bg-cover bg-center items-center rounded-md"
          :style="{
            backgroundImage:
              'url(' + require(`~/assets/images/${images[index]}.jpg`) + ')',
          }"
          style="height: 32rem; width: 34rem"
        >
          <!-- Controls -->
          <!--  Close button -->
          <button
            class="absolute top-0 right-0 -mt-8 -ml-3 mx-2"
            @click="modalOpen = false"
          >
            <svg
              class="control"
              width="14"
              height="15"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="m11.596.782 2.122 2.122L9.12 7.499l4.597 4.597-2.122 2.122L7 9.62l-4.595 4.597-2.122-2.122L4.878 7.5.282 2.904 2.404.782l4.595 4.596L11.596.782Z"
                fill="#FFFFFF"
                fill-rule="evenodd"
              />
            </svg>
          </button>

          <div class="w-full flex justify-between">
            <button
              class="-ml-6 mx-2 btn btn-circle btn-md bg-white hover:bg-white border-0"
              @click="index == 0 ? (index = images.length - 1) : index--"
            >
              <svg
                class="control"
                xmlns="http://www.w3.org/2000/svg"
                width="16"
                height="16"
                viewBox="0 0 16 16"
              >
                <path
                  fill-rule="evenodd"
                  d="M11.354 1.646a.5.5 0 0 1 0 .708L5.707 8l5.647 5.646a.5.5 0 0 1-.708.708l-6-6a.5.5 0 0 1 0-.708l6-6a.5.5 0 0 1 .708 0z"
                />
              </svg>
            </button>
            <button
              class="-mr-6 mx-2 btn btn-circle btn-md bg-white hover:bg-white border-0"
              @click="index + 1 == images.length ? (index = 0) : index++"
            >
              <svg
                class="control"
                xmlns="http://www.w3.org/2000/svg"
                width="16"
                height="16"
                viewBox="0 0 16 16"
              >
                <path
                  fill-rule="evenodd"
                  d="M4.646 1.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1 0 .708l-6 6a.5.5 0 0 1-.708-.708L10.293 8 4.646 2.354a.5.5 0 0 1 0-.708z"
                />
              </svg>
            </button>
          </div>
        </div>
        <div class="flex justify-center w-full mt-3 space-x-4">
          <div class="image-list" @click.capture="index = 0">
            <img class="h-24" src="~/assets/images/image-product-1-thumbnail.jpg" />
          </div>
          <div class="image-list" @click.capture="index = 1">
            <img class="h-24" src="~/assets/images/image-product-2-thumbnail.jpg" />
          </div>
          <div class="image-list" @click.capture="index = 2">
            <img class="h-24" src="~/assets/images/image-product-3-thumbnail.jpg" />
          </div>
          <div class="image-list" @click.capture="index = 3">
            <img class="h-24" src="~/assets/images/image-product-4-thumbnail.jpg" />
          </div>
        </div>
      </div>
    </div>
    <!-- Drawer-->
    <Drawer v-if="isMobile" :direction="'left'" :exist="true" ref="LeftDrawer">
      <div class="px-3 py-4">
        <nav-links :is-mobile="isMobile"
          ><li>
            <a @click="close">
              <svg width="14" height="15" xmlns="http://www.w3.org/2000/svg">
                <path
                  d="m11.596.782 2.122 2.122L9.12 7.499l4.597 4.597-2.122 2.122L7 9.62l-4.595 4.597-2.122-2.122L4.878 7.5.282 2.904 2.404.782l4.595 4.596L11.596.782Z"
                  fill="#69707D"
                  fill-rule="evenodd"
                />
              </svg>
            </a></li
        ></nav-links>
      </div>
    </Drawer>
  </div>
</template>
<script>
export default {
  data() {
    return {
      index: 0,
      windowWidth: null,
      isMobile: false,
      price: 125,
      cartCount: 0,
      modalOpen: false,
      images: [
        "image-product-1",
        "image-product-2",
        "image-product-3",
        "image-product-4",
      ],
    };
  },
  computed: {
    classObject: function () {
      if (!this.isMobile) {
        return ["product-img"];
      }

      return [];
    },
  },
  watch: {
    windowWidth() {
      this.onResize();
    },
  },
  methods: {
    openMenu() {
      if (this.$refs.LeftDrawer.active) {
        this.$refs.LeftDrawer.close();
      } else {
        this.$refs.LeftDrawer.open();
      }
    },
    close() {
      this.$refs.LeftDrawer.close();
    },

    onResize() {
      this.windowWidth = window.innerWidth;
      this.isMobile = this.windowWidth < 760 ? true : false;
    },

    showModal() {
      //only show modal in big screens
      this.modalOpen = true;
      /*  if (this.windowWidth < 1280) {
        //dont show modal or render it un clickable
      } */
    },
  },

  mounted() {
    this.$nextTick(() => {
      this.onResize();
    });
    window.addEventListener("resize", this.onResize);
  },
  beforeDestroy() {
    window.removeEventListener("resize", this.onResize);
  },
};
</script>
<style>
html {
  font-family: "Kumbh Sans";
  font-weight: 700;
}

.i-primary {
  color: hsl(26, 100%, 55%);
}

.i-primary-bg {
  background-color: hsl(26, 100%, 55%);
}

.bg-pale-primary {
  background-color: hsl(25, 100%, 94%);
}

.btn-i-primary {
  @apply i-primary-bg border-0 text-white;
}

.btn-i-primary:hover,
.btn-i-primary:active {
  background-color: hsl(26, 100%, 55%);
  opacity: 0.5;
}

.i-primary-shadow {
  @apply shadow-3xl-orange;
}

.product-img {
  height: 28rem;
  @apply rounded-md;
}

.image-list {
  @apply relative;
  cursor: pointer;
}

.image-list > img {
  z-index: 1;
  @apply border-0 rounded-md;
}

.avatar:hover {
  @apply rounded-full border-2;
  border-color: hsl(26, 100%, 55%);
}
.image-list:hover::after {
  position: absolute;
  content: "";
  background-color: rgb(253 253 253 / 64%);
  @apply w-full h-full inset-0 border-2 rounded-md;
  border-color: hsl(26, 100%, 55%);
  z-index: 2;
}

svg.control:hover {
  color: hsl(26, 100%, 55%);
}
</style>
