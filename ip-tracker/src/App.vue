<template>
  <header class="pattern-bg">
    <div class="container mx-auto pt-4 pb-16">
      <h1 class="font-bold text-2xl text-white text-center pb-4">IP Address Tracker</h1>
      <div class="flex justify-center pb-6">
        <input placeholder="Search for any IP address or domain" class="rounded-l-xl px-6 w-2/6 text-sm" type="text">
        <button class="bg-black p-4 flex justity-center rounded-r-xl">
          <img src="./assets/icon-arrow.svg" alt="click here to search!" />
        </button>
      </div>
    </div>
  </header>

  <main class="relative">
    <div class="grid grid-cols-4 w-3/5 rounded-lg py-6 px-5 bg-white drop-shadow-lg absolute -top-12 left-1/2 -translate-x-2/4">
      <div class="border-r">
        <h2>ip address</h2>
        <div class="font-bold">{{ count }}</div>
      </div>
      <div class="border-r px-4">
        <h2>location</h2>
        <div class="font-bold">area name</div>
      </div>
      <div class="border-r">
        <h2>timezone</h2>
        <div class="font-bold">utc</div>
      </div>
      <div>
        <h2>isp</h2>
        <div class="font-bold">unifi</div>
      </div>
    </div>
    <div class="container">
      <div class="font-bold">Map Here</div>
    </div>
  </main>
</template>

<script>
export default {
  setup() {
    const count = 0

    return {
      count
    }
  }
}
</script>
