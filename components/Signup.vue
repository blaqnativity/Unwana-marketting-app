<template>
  <form class="w-1/3 mx-auto shadow space-y-4 p-6 rounded-md" @submit.prevent>
    <!-- input group -->
    <div class="inputGroup flex flex-col space-y-2 items-start">
      <label for="">Full name</label>
      <input class="w-full" type="text" placeholder="Mark Williams" />
    </div>
    <!-- input group -->
    <div class="inputGroup flex flex-col space-y-2 items-start">
      <label for="">Email</label>
      <input
        class="w-full"
        type="email"
        placeholder="markwilliams@outlook.com"
      />
    </div>
    <!-- input group -->
    <div class="inputGroup flex flex-col space-y-2 items-start">
      <label for="">Password</label>
      <input
        class="w-full"
        type="password"
        placeholder="8+ characters required"
      />
    </div>
    <!-- input group -->
    <div class="inputGroup flex flex-col space-y-2 items-start">
      <label for="">Phone</label>
      <input class="w-full" type="value" placeholder="+234569****" />
    </div>
    <!-- input group -->
    <div class="inputGroup flex space-x-2 items-center">
      <label for="">Accept terms</label>
      <input type="checkbox" />
    </div>

    <button class="btnMain">Create Account</button>
  </form>
</template>
