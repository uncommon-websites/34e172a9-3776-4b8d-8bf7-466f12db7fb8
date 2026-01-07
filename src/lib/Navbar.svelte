<script lang="ts">
  import Button from './Button.svelte';
  
  let isMenuOpen = false;
</script>

<nav class="fixed top-0 left-0 right-0 z-50 bg-cream/90 backdrop-blur-sm border-b border-gray-200/50">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex justify-between items-center h-20">
      <!-- Logo -->
      <div class="flex-shrink-0 flex items-center">
        <a href="/" class="flex items-center gap-2">
          <!-- WC26 Logo Icon -->
          <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
            <circle cx="16" cy="16" r="16" fill="#191817"/>
            <path d="M16 8L20 14H12L16 8Z" fill="white"/>
            <path d="M16 24L12 18H20L16 24Z" fill="white"/>
            <circle cx="16" cy="16" r="3" fill="oklch(0.656 0.241 354.308)"/>
          </svg>
          <span class="font-bold text-xl tracking-tight">WC26</span>
        </a>
      </div>

      <!-- Desktop Navigation -->
      <div class="hidden md:flex items-center space-x-8">
        <a href="#simulator" class="text-sm font-medium hover:text-orange-brand transition-colors">Simulator</a>
        <a href="#community" class="text-sm font-medium hover:text-orange-brand transition-colors">The Club</a>
        <a href="#analytics" class="text-sm font-medium hover:text-orange-brand transition-colors">Analytics</a>
      </div>

      <!-- Right Side -->
      <div class="hidden md:flex items-center space-x-6">
        <a href="#" class="text-sm font-medium hover:text-orange-brand transition-colors">About</a>
        <a href="#" class="text-sm font-medium hover:text-orange-brand transition-colors">Login</a>
        <Button href="#" className="!py-2 !px-4 !text-sm">Join Waitlist &rarr;</Button>
      </div>

      <!-- Mobile menu button -->
      <div class="md:hidden flex items-center">
        <button on:click={() => isMenuOpen = !isMenuOpen} class="text-gray-600 hover:text-gray-900 focus:outline-none">
          <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </button>
      </div>
    </div>
  </div>
</nav>
