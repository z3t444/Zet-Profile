<template>
  <div class="mt-80">
    <div class="ClassName text-center">
      <h3 class="text-4xl font-medium">You can leave a message below</h3>
      <p class="xl:w-1/4 mx-auto mt-5 text-gray-700">Tell me whatever it is. give us the best message so that we are more enthusiastic to work.</p>
    </div>
    <div class="mt-20">
      <form action="https://api.web3forms.com/submit" method="POST" class="grid gap-4 max-w-5xl mx-auto p-4 rounded-lg">
        <input type="hidden" name="access_key" value="3a928331-13f9-4e84-86cf-adb4fb41d57e" />
        <div class="flex items-center gap-4">
          <input type="text" name="name" required placeholder="Your Name" class="w-full px-3 py-2 rounded-xl shadow-lg focus:outline-none bg-transparent focus:border-blue-500" />
          <input type="email" name="email" required placeholder="Your Email" class="w-full px-3 py-2 rounded-xl shadow-lg focus:outline-none bg-transparent focus:border-blue-500" />
        </div>
        <textarea name="message" required placeholder="Your Message" class="w-full px-3 py-2 h-40 rounded-xl shadow-lg focus:outline-none bg-transparent focus:border-blue-500"></textarea>
        <button type="submit" class=" w-48 mx-auto mt-10 py-2 px-4 text-sm bg-gray-900 text-white font-semibold rounded-xl hover:bg-blue-600 focus:outline-none duration-100 focus:bg-blue-600">Submit Form</button>
      </form>
    </div>
  </div>
</template>
