<script>
  import "../app.css";
</script>
<!-- Planned colors:
🌸 Blush Pink (#F4C6C3)
🥛 Ivory Cream (#FAF3E0)
🌿 Sage Green (#A8B5A2) - Accents
🎀 Antique Rose (#D59A9A) 
Primary Text Colors
  🖤 Deep Charcoal (#3C3C3C) – A soft black, great for main text.
  ☕ Warm Mocha Brown (#8D6A5E) – A warm coffee-like brown.
  🍇 Muted Plum (#70525A) – A subtle vintage purple.
  🍂 Classic Espresso (#5C4033) – A rich brown with old-world charm.
  🌿 Dark Sage (#5A6B5A) – A muted green-gray for an earthy feel.
Background & Highlight Colors
  🕊 Ivory Cream (#FAF3E0) – A soft, elegant off-white.
  🎗 Soft Beige (#EFE7DA) – A warm, vintage beige.
  🌷 Antique Rose (#D59A9A) – A delicate pink with nostalgia.
Accent Colors (For Links & Buttons)
  🍷 Vintage Burgundy (#703D46) – A deep, romantic wine red.
  ✨ Dusty Gold (#BFA17F) – An aged, elegant gold hue.
-->
<nav class="bg-antique-rose border-sage-green border-b-4">
  <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
    <a href="https://youtu.be/dQw4w9WgXcQ" class="flex items-center space-x-3 rtl:space-x-reverse">
        <span class="self-center text-2l font-semibold whitespace-nowrap text-dark-sage">California Vintage Clothes</span>
    </a>
    <button data-collapse-toggle="navbar-default" type="button" class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="navbar-default" aria-expanded="false">
        <span class="sr-only">Open main menu</span>
        <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1h15M1 7h15M1 13h15"/>
        </svg>
    </button>
    <div class="hidden w-full md:block md:w-auto" id="navbar-default">
      <ul class="font-medium flex flex-col p-4 md:p-0 mt-4 border-2 border-warm-mocha-brown rounded-lg bg-antique-rose md:flex-row md:space-x-8 rtl:space-x-reverse md:mt-0 md:border-0 md:bg-antique-rose">
        <li>
          <a href="#" class="block py-2 px-3 text-deep-charcoal bg-ivory-cream rounded-sm md:bg-transparent md:text-dark-sage md:p-0 " aria-current="page">Home</a>
        </li>
        <li>
          <a href="#" class="block py-2 px-3 text-white rounded-sm hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-dark-sage md:p-0">About</a>
        </li>
        <li>
          <a href="#" class="block py-2 px-3 text-white rounded-sm hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-dark-sage md:p-0 ">Services</a>
        </li>
        <li>
          <a href="#" class="block py-2 px-3 text-white rounded-sm hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-dark-sage md:p-0 ">Pricing</a>
        </li>
        <li>
          <a href="#" class="block py-2 px-3 text-white rounded-sm hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-dark-sage md:p-0 ">Contact</a>
        </li>
      </ul>
    </div>
  </div>
</nav>

<slot />