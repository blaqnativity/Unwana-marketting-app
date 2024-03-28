<template>
  <form class="w-1/3 mx-auto shadow space-y-4 p-6 rounded-md" @submit.prevent>
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

    <button class="btnMain">Sign in</button>
  </form>
</template>
