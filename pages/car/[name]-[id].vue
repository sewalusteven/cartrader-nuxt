<template>
    <div>
     <!-- CAR DETAIL PAGE -->
    <div
    class="mx-auto mt-4 max-w-7xl space-y-4 px-4 xs:px-8 sm:px-10 lg:px-16 pb-16 w-3/5"
    >

      <CarDetailHero />
      <CarDetailAttributes />
    <!-- CAR DESCRISPTION -->
    <div class="mt-5">
      <p class="mb-10">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Exercitationem
        consequuntur, et saepe sequi, ipsum quisquam iste autem quas vel aperiam
        laboriosam dolorum vero tempore placeat, asperiores alias magni. Nulla,
        dolores.
      </p>
    </div>
    <!-- CAR DESCRISPTION -->
    <!-- CAR CONTACT -->
    <div class="mt-10">
      <div class="flex w-[600px] justify-between">
        <input type="text" class="border p-1" placeholder="Name" />
        <input type="text" class="border p-1" placeholder="Email" />
        <input type="text" class="border p-1" placeholder="Phone" />
      </div>
      <div class="flex mt-4 w-[600px]">
        <textarea class="border p-1 w-full" placeholder="Message"></textarea>
      </div>
      <button class="bg-blue-400 text-white px-10 py-3 rounded mt-4">
        Submit
      </button>
    </div>
    <!-- CAR CONTACT -->
    </div>
    <!-- CAR DETAIL PAGE   -->
    </div>
</template>
<script setup>
const route =  useRoute();
useHead({
  title: route.params.name.toUpperCase()
})
</script>