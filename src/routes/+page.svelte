<script lang="ts">
  import Navbar from '$lib/Navbar.svelte';
  import Footer from '$lib/Footer.svelte';
  import Button from '$lib/Button.svelte';
</script>

<div class="min-h-screen font-sans text-dark bg-cream overflow-x-hidden">
  <Navbar />

  <!-- Hero Section -->
  <section class="pt-32 pb-16 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto text-center">
    <div class="mb-6">
      <span class="text-xs font-bold tracking-widest text-gray-500 uppercase">World Cup 2026 • USA • Canada • Mexico</span>
    </div>
    <h1 class="text-5xl md:text-7xl font-serif mb-6 leading-tight">
      Your nation's journey <br class="hidden md:block" /> starts here
    </h1>
    <p class="text-lg md:text-xl text-gray-600 max-w-2xl mx-auto mb-10 leading-relaxed">
      The complete coordination platform for World Cup fans. Simulate tournament paths, connect with your nation's community, and never miss a once-in-a-lifetime moment.
    </p>
    <div class="flex flex-col sm:flex-row items-center justify-center gap-4 mb-20">
      <Button href="#" type="primary">Join Waitlist &rarr;</Button>
      <Button href="#" type="outline">Explore Simulator</Button>
    </div>

    <!-- Hero Image -->
    <div class="relative w-full max-w-5xl mx-auto rounded-2xl overflow-hidden shadow-2xl border border-gray-200 bg-white aspect-[16/9] mb-16 group">
      <!-- Hero Background Image -->
      <img src="/generated/image-diverse-group-of-passionate-football-fan-1767812741797-0.webp" alt="World Cup fans celebrating" class="absolute inset-0 w-full h-full object-cover" />
      <!-- Overlay with Tournament Bracket UI -->
      <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-black/40 to-transparent p-6">
        <div class="h-full w-full bg-white rounded-xl border border-gray-200 shadow-sm p-6 flex flex-col">
            <!-- Header -->
            <div class="flex items-center justify-between mb-6 border-b border-gray-100 pb-4">
                <div class="flex items-center gap-3">
                    <div class="font-bold text-lg">🏆 World Cup 2026 Simulator</div>
                </div>
                <div class="flex gap-2">
                    <div class="px-3 py-1.5 bg-orange-brand/10 text-orange-brand rounded-lg text-xs font-bold">Your Team: Argentina</div>
                </div>
            </div>
            <!-- Tournament Bracket Mockup -->
            <div class="flex-1 flex items-center justify-center gap-8">
                <!-- Round of 16 -->
                <div class="space-y-4">
                    <div class="bg-gray-50 p-3 rounded-lg border border-gray-200 w-32">
                        <div class="text-xs font-bold mb-1">Round of 16</div>
                        <div class="flex items-center gap-2 text-xs">
                            <span>🇦🇷</span>
                            <span class="font-medium">ARG</span>
                        </div>
                    </div>
                    <div class="bg-gray-50 p-3 rounded-lg border border-gray-200 w-32 opacity-50">
                        <div class="h-3 w-16 bg-gray-200 rounded mb-1"></div>
                        <div class="h-2 w-12 bg-gray-200 rounded"></div>
                    </div>
                </div>
                <!-- Quarter Finals -->
                <div class="space-y-8">
                    <div class="bg-orange-brand/10 p-3 rounded-lg border-2 border-orange-brand w-32">
                        <div class="text-xs font-bold mb-1 text-orange-brand">Quarter Final</div>
                        <div class="flex items-center gap-2 text-xs">
                            <span>🇦🇷</span>
                            <span class="font-medium">ARG</span>
                        </div>
                    </div>
                </div>
                <!-- Semi Finals -->
                <div class="space-y-12">
                    <div class="bg-gray-50 p-3 rounded-lg border border-gray-200 w-32">
                        <div class="text-xs font-bold mb-1">Semi Final</div>
                        <div class="h-2 w-12 bg-gray-200 rounded"></div>
                    </div>
                </div>
                <!-- Final -->
                <div>
                    <div class="bg-gray-50 p-3 rounded-lg border border-gray-200 w-32">
                        <div class="text-xs font-bold mb-1">🏆 Final</div>
                        <div class="h-2 w-12 bg-gray-200 rounded"></div>
                    </div>
                </div>
            </div>
        </div>
      </div>
      
      <!-- Decorative Elements -->
      <div class="absolute -left-12 bottom-12 w-24 h-24 bg-orange-brand rounded-full blur-2xl opacity-20"></div>
      <div class="absolute -right-12 top-12 w-32 h-32 bg-orange-brand rounded-full blur-2xl opacity-20"></div>

      <!-- Football Icon -->
      <div class="absolute bottom-[-20px] left-[-40px] w-32 h-32 z-10 hidden md:block">
          <svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
            <circle cx="50" cy="50" r="40" fill="white" stroke="#191817" stroke-width="2"/>
            <path d="M50 20 L60 40 L50 45 L40 40 Z" fill="#191817"/>
            <path d="M30 35 L40 40 L35 55 L20 50 Z" fill="#191817"/>
            <path d="M70 35 L80 50 L65 55 L60 40 Z" fill="#191817"/>
            <path d="M35 55 L50 45 L65 55 L60 70 L40 70 Z" fill="#191817"/>
            <path d="M25 65 L40 70 L35 80 L20 75 Z" fill="#191817"/>
            <path d="M75 65 L80 75 L65 80 L60 70 Z" fill="#191817"/>
          </svg>
      </div>
    </div>

    <!-- Stats -->
    <div class="text-center">
      <p class="text-sm text-gray-500 mb-6">Built for the biggest sporting event on the planet</p>
      <div class="flex flex-wrap justify-center items-center gap-8 md:gap-12">
        <div class="text-center">
          <div class="text-3xl font-serif font-bold text-dark">48</div>
          <div class="text-xs text-gray-500 uppercase tracking-wider">Teams</div>
        </div>
        <div class="text-center">
          <div class="text-3xl font-serif font-bold text-dark">16</div>
          <div class="text-xs text-gray-500 uppercase tracking-wider">Host Cities</div>
        </div>
        <div class="text-center">
          <div class="text-3xl font-serif font-bold text-dark">104</div>
          <div class="text-xs text-gray-500 uppercase tracking-wider">Matches</div>
        </div>
        <div class="text-center">
          <div class="text-3xl font-serif font-bold text-dark">10,000+</div>
          <div class="text-xs text-gray-500 uppercase tracking-wider">Possible Paths</div>
        </div>
      </div>
    </div>
  </section>

  <!-- Stats Section -->
  <section id="simulator" class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16 max-w-3xl mx-auto">
        Three pillars to transform your World Cup experience
      </h2>
      
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-16">
        <div class="bg-gray-50 p-8 rounded-2xl text-center">
          <div class="text-4xl font-serif font-medium mb-2">🎯 Simulator</div>
          <div class="text-sm text-gray-600 mt-4">Explore 10,000+ tournament paths before they happen</div>
        </div>
        <div class="bg-gray-50 p-8 rounded-2xl text-center">
          <div class="text-4xl font-serif font-medium mb-2">🤝 The Club</div>
          <div class="text-sm text-gray-600 mt-4">Nation-based communities to coordinate everything</div>
        </div>
        <div class="bg-gray-50 p-8 rounded-2xl text-center">
          <div class="text-4xl font-serif font-medium mb-2">📊 Analytics</div>
          <div class="text-sm text-gray-600 mt-4">Track your team's performance and tactical insights</div>
        </div>
      </div>

      <!-- Nation Communities Carousel -->
      <div class="flex gap-4 overflow-hidden relative">
        <div class="absolute inset-y-0 left-0 w-20 bg-gradient-to-r from-white to-transparent z-10"></div>
        <div class="absolute inset-y-0 right-0 w-20 bg-gradient-to-l from-white to-transparent z-10"></div>
        
        <div class="flex gap-4 animate-scroll">
            <!-- Card 1 - Argentina -->
            <div class="w-64 h-80 bg-gradient-to-br from-blue-100 to-blue-200 rounded-2xl flex-shrink-0 relative overflow-hidden group">
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-3 py-1.5 rounded-full text-sm font-bold flex items-center gap-2">
                    🇦🇷 Argentina
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-black/80 to-transparent p-6 text-white">
                    <div class="font-bold text-lg mb-2">La Albiceleste</div>
                    <div class="text-xs opacity-90 mb-3">Defending Champions • 3 Stars</div>
                    <div class="flex gap-2 text-xs">
                        <span class="bg-white/20 px-2 py-1 rounded">2.4K Members</span>
                        <span class="bg-white/20 px-2 py-1 rounded">Active</span>
                    </div>
                </div>
            </div>
            <!-- Card 2 - Brazil -->
            <div class="w-64 h-80 bg-gradient-to-br from-green-100 to-yellow-100 rounded-2xl flex-shrink-0 relative overflow-hidden group">
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-3 py-1.5 rounded-full text-sm font-bold flex items-center gap-2">
                    🇧🇷 Brazil
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-black/80 to-transparent p-6 text-white">
                    <div class="font-bold text-lg mb-2">Seleção</div>
                    <div class="text-xs opacity-90 mb-3">5-Time Champions • Record Holders</div>
                    <div class="flex gap-2 text-xs">
                        <span class="bg-white/20 px-2 py-1 rounded">3.1K Members</span>
                        <span class="bg-white/20 px-2 py-1 rounded">Active</span>
                    </div>
                </div>
            </div>
            <!-- Card 3 - USA -->
            <div class="w-64 h-80 bg-gradient-to-br from-red-100 to-blue-100 rounded-2xl flex-shrink-0 relative overflow-hidden group">
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-3 py-1.5 rounded-full text-sm font-bold flex items-center gap-2">
                    🇺🇸 USA
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-black/80 to-transparent p-6 text-white">
                    <div class="font-bold text-lg mb-2">USMNT</div>
                    <div class="text-xs opacity-90 mb-3">Host Nation • Home Advantage</div>
                    <div class="flex gap-2 text-xs">
                        <span class="bg-white/20 px-2 py-1 rounded">5.2K Members</span>
                        <span class="bg-white/20 px-2 py-1 rounded">Active</span>
                    </div>
                </div>
            </div>
             <!-- Card 4 - England -->
            <div class="w-64 h-80 bg-gradient-to-br from-white to-red-100 rounded-2xl flex-shrink-0 relative overflow-hidden group">
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-3 py-1.5 rounded-full text-sm font-bold flex items-center gap-2">
                    🏴󠁧󠁢󠁥󠁮󠁧󠁿 England
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-black/80 to-transparent p-6 text-white">
                    <div class="font-bold text-lg mb-2">Three Lions</div>
                    <div class="text-xs opacity-90 mb-3">1966 Champions • Coming Home?</div>
                    <div class="flex gap-2 text-xs">
                        <span class="bg-white/20 px-2 py-1 rounded">4.7K Members</span>
                        <span class="bg-white/20 px-2 py-1 rounded">Active</span>
                    </div>
                </div>
            </div>
             <!-- Card 5 - Mexico -->
            <div class="w-64 h-80 bg-gradient-to-br from-green-200 to-red-200 rounded-2xl flex-shrink-0 relative overflow-hidden group">
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-3 py-1.5 rounded-full text-sm font-bold flex items-center gap-2">
                    🇲🇽 Mexico
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-black/80 to-transparent p-6 text-white">
                    <div class="font-bold text-lg mb-2">El Tri</div>
                    <div class="text-xs opacity-90 mb-3">Host Nation • Passionate Support</div>
                    <div class="flex gap-2 text-xs">
                        <span class="bg-white/20 px-2 py-1 rounded">6.8K Members</span>
                        <span class="bg-white/20 px-2 py-1 rounded">Active</span>
                    </div>
                </div>
            </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Problem Section -->
  <section class="bg-dark text-white py-24 overflow-hidden">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-4">The World Cup coordination <br /> problem</h2>
      <p class="text-center text-gray-400 mb-16">Traveling fans face chaos without a coordination platform</p>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
        <!-- The Problem -->
        <div>
          <h3 class="text-xl font-serif mb-2">Without WC26</h3>
          <p class="text-gray-400 text-sm mb-8 leading-relaxed">
            Fans spend thousands following their team, but miss incredible moments because coordination doesn't exist. Information is scattered across Reddit, WhatsApp, and Telegram.
          </p>
          <div class="bg-gray-800/50 rounded-xl p-6 border border-gray-700 relative">
             <div class="space-y-3">
                <div class="flex items-center gap-3 text-sm">
                    <div class="w-8 h-8 bg-red-500/20 rounded flex items-center justify-center text-red-400">✗</div>
                    <span class="text-gray-300">Missed 100+ fan moments</span>
                </div>
                <div class="flex items-center gap-3 text-sm">
                    <div class="w-8 h-8 bg-red-500/20 rounded flex items-center justify-center text-red-400">✗</div>
                    <span class="text-gray-300">Paid $10K+ unnecessarily</span>
                </div>
                <div class="flex items-center gap-3 text-sm">
                    <div class="w-8 h-8 bg-red-500/20 rounded flex items-center justify-center text-red-400">✗</div>
                    <span class="text-gray-300">Fragmented information</span>
                </div>
                <div class="flex items-center gap-3 text-sm">
                    <div class="w-8 h-8 bg-red-500/20 rounded flex items-center justify-center text-red-400">✗</div>
                    <span class="text-gray-300">No planning tools</span>
                </div>
                <div class="flex items-center gap-3 text-sm">
                    <div class="w-8 h-8 bg-red-500/20 rounded flex items-center justify-center text-red-400">✗</div>
                    <span class="text-gray-300">Alone in the chaos</span>
                </div>
             </div>
          </div>
        </div>

        <!-- The Solution -->
        <div>
          <h3 class="text-xl font-serif mb-2">With WC26</h3>
          <p class="text-gray-400 text-sm mb-8 leading-relaxed">
            One platform to simulate paths, coordinate with your nation's community, split costs, and never miss a moment. Save thousands while experiencing it all.
          </p>
          <div class="bg-gray-800/50 rounded-xl p-6 border border-green-500/30 relative">
             <div class="space-y-3">
                <div class="flex items-center gap-3 text-sm">
                    <div class="w-8 h-8 bg-green-500/20 rounded flex items-center justify-center text-green-400">✓</div>
                    <span class="text-gray-300">Plan every possible scenario</span>
                </div>
                <div class="flex items-center gap-3 text-sm">
                    <div class="w-8 h-8 bg-green-500/20 rounded flex items-center justify-center text-green-400">✓</div>
                    <span class="text-gray-300">Split Airbnbs & save thousands</span>
                </div>
                <div class="flex items-center gap-3 text-sm">
                    <div class="w-8 h-8 bg-green-500/20 rounded flex items-center justify-center text-green-400">✓</div>
                    <span class="text-gray-300">Nation-based coordination</span>
                </div>
                <div class="flex items-center gap-3 text-sm">
                    <div class="w-8 h-8 bg-green-500/20 rounded flex items-center justify-center text-green-400">✓</div>
                    <span class="text-gray-300">Real-time team intel</span>
                </div>
                <div class="flex items-center gap-3 text-sm">
                    <div class="w-8 h-8 bg-green-500/20 rounded flex items-center justify-center text-green-400">✓</div>
                    <span class="text-gray-300">Never travel alone</span>
                </div>
             </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Features Section 1 -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16 max-w-2xl mx-auto">
        Everything you need to coordinate your World Cup journey
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <!-- Card 1: Tournament Simulator -->
        <div class="lg:col-span-2 bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden relative group">
            <div class="mb-8">
                <h3 class="text-xl font-serif mb-2">🎯 Tournament Simulator</h3>
                <p class="text-gray-500 text-sm">Explore all 10,000+ possible tournament paths before they happen. Plan which cities to book, which tickets to buy, which matches your team might play.</p>
            </div>
            <div class="bg-red-50 rounded-xl p-6 h-64 relative border border-red-100">
                <!-- Bracket Visualization -->
                <div class="flex items-center justify-around h-full">
                    <div class="text-center">
                        <div class="text-2xl mb-2">🇦🇷</div>
                        <div class="text-xs font-bold">Argentina</div>
                        <div class="text-[10px] text-gray-400">Group A</div>
                    </div>
                    <div class="flex flex-col gap-2">
                        <div class="w-16 h-0.5 bg-gray-300"></div>
                        <div class="w-16 h-0.5 bg-gray-300"></div>
                    </div>
                    <div class="bg-white p-3 rounded-lg shadow-sm">
                        <div class="text-xs font-bold mb-1">R16 Match</div>
                        <div class="text-[10px] text-gray-500">Miami</div>
                    </div>
                    <div class="flex flex-col gap-2">
                        <div class="w-16 h-0.5 bg-orange-brand"></div>
                    </div>
                    <div class="bg-orange-brand/10 p-3 rounded-lg border-2 border-orange-brand">
                        <div class="text-xs font-bold mb-1 text-orange-brand">Quarter</div>
                        <div class="text-[10px] text-gray-600">Dallas</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Card 2: Nation Communities -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden">
            <div class="mb-8">
                <h3 class="text-xl font-serif mb-2">🤝 Nation Communities</h3>
                <p class="text-gray-500 text-sm">Connect with fans from your nation. Split Airbnbs, organize carpools, find watch parties, and coordinate everything.</p>
            </div>
            <div class="bg-blue-50 rounded-xl h-48 relative overflow-hidden flex items-center justify-center">
                <div class="flex gap-2 flex-wrap justify-center p-4">
                    <span class="bg-white px-3 py-1.5 rounded-lg shadow-sm text-xs font-medium">🇦🇷 Argentina</span>
                    <span class="bg-white px-3 py-1.5 rounded-lg shadow-sm text-xs font-medium">🇧🇷 Brazil</span>
                    <span class="bg-white px-3 py-1.5 rounded-lg shadow-sm text-xs font-medium">🇺🇸 USA</span>
                    <span class="bg-white px-3 py-1.5 rounded-lg shadow-sm text-xs font-medium">🏴󠁧󠁢󠁥󠁮󠁧󠁿 England</span>
                    <span class="bg-white px-3 py-1.5 rounded-lg shadow-sm text-xs font-medium">🇲🇽 Mexico</span>
                    <span class="bg-white px-3 py-1.5 rounded-lg shadow-sm text-xs font-medium">🇫🇷 France</span>
                </div>
            </div>
        </div>

        <!-- Card 3: Split Costs -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden">
             <div class="h-48 bg-green-50 rounded-xl mb-6 p-4 relative flex items-center justify-center">
                <div class="bg-white rounded-xl shadow-lg p-4 w-full max-w-[200px]">
                    <div class="text-xs font-bold mb-3 text-center">Miami Airbnb</div>
                    <div class="flex items-center justify-between mb-2">
                        <span class="text-xs text-gray-500">Total:</span>
                        <span class="text-sm font-bold line-through text-gray-400">$2,400</span>
                    </div>
                    <div class="flex items-center justify-between">
                        <span class="text-xs text-gray-500">Split 6 ways:</span>
                        <span class="text-lg font-bold text-green-600">$400</span>
                    </div>
                    <div class="mt-3 pt-3 border-t border-gray-100">
                        <div class="text-[10px] text-gray-400 text-center">Save $2,000 per person</div>
                    </div>
                </div>
             </div>
             <h3 class="text-xl font-serif mb-2">Split costs & save thousands</h3>
             <p class="text-gray-500 text-sm">Share Airbnbs, organize carpools, and coordinate group activities to drastically reduce your World Cup expenses.</p>
        </div>

        <!-- Card 4: Real-Time Intel -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden">
             <div class="h-48 bg-orange-50 rounded-xl mb-6 p-4 flex items-center justify-center">
                <div class="bg-white p-4 rounded-xl shadow-sm w-full max-w-[200px] space-y-2">
                    <div class="flex items-center gap-2 text-xs">
                        <div class="w-2 h-2 bg-green-500 rounded-full animate-pulse"></div>
                        <span class="font-bold">Team spotted at hotel</span>
                    </div>
                    <div class="text-[10px] text-gray-500">Training at 3pm - Stadium B</div>
                    <div class="flex items-center gap-2 text-xs mt-3">
                        <div class="w-2 h-2 bg-orange-500 rounded-full"></div>
                        <span class="font-bold">Watch party organized</span>
                    </div>
                    <div class="text-[10px] text-gray-500">Downtown Miami - 200+ fans</div>
                </div>
             </div>
             <h3 class="text-xl font-serif mb-2">Real-time team intel</h3>
             <p class="text-gray-500 text-sm">Get live updates on team sightings, training schedules, watch parties, and fan rallies—never miss a moment.</p>
        </div>

        <!-- Card 5: Analytics -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden">
             <div class="h-48 bg-purple-50 rounded-xl mb-6 p-4 flex items-center justify-center relative">
                 <div class="bg-white p-4 rounded-xl shadow-sm w-full max-w-[220px]">
                    <div class="text-xs font-bold mb-3">📊 Argentina Stats</div>
                    <div class="space-y-2">
                        <div class="flex justify-between text-xs">
                            <span class="text-gray-500">Goals Scored</span>
                            <span class="font-bold">12</span>
                        </div>
                        <div class="flex justify-between text-xs">
                            <span class="text-gray-500">Possession</span>
                            <span class="font-bold">58%</span>
                        </div>
                        <div class="flex justify-between text-xs">
                            <span class="text-gray-500">Win Probability</span>
                            <span class="font-bold text-green-600">72%</span>
                        </div>
                    </div>
                 </div>
             </div>
             <h3 class="text-xl font-serif mb-2">Team analytics & insights</h3>
             <p class="text-gray-500 text-sm">Track your team's performance, tactical breakdowns, opponent analysis, and qualification scenarios.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Testimonial 1 -->
  <section class="py-16 bg-cream">
    <div class="max-w-4xl mx-auto px-4 text-center">
        <div class="flex justify-center mb-8">
            <div class="text-4xl">🇦🇷</div>
        </div>
        <blockquote class="text-2xl md:text-3xl font-serif leading-relaxed mb-8">
            "I spent $10,000 following Argentina through Qatar 2022. The experience was incredible, but I missed 100+ moments because coordination didn't exist. WC26 solves this—I'll never travel alone again."
        </blockquote>
        <div class="flex items-center justify-center gap-4">
            <img src="/generated/image-portrait-of-an-enthusiastic-male-footbal-1767812750874-3.webp" alt="Karn Saxena" class="w-12 h-12 rounded-full object-cover" />
            <div class="text-left">
                <div class="font-bold text-sm">Karn Saxena</div>
                <div class="text-xs text-gray-500">Founder & CEO, WC26</div>
            </div>
        </div>
    </div>
  </section>

  <!-- Features Section 2 -->
  <section id="community" class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16">
        Coordinate everything <br /> with your nation's community
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <!-- Card 1 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="bg-blue-50 rounded-xl h-64 mb-8 p-4 relative overflow-hidden flex items-center justify-center">
                <!-- Community Feed Mockup -->
                <div class="w-full max-w-sm space-y-3">
                    <div class="bg-white p-3 rounded-lg shadow-sm">
                        <div class="flex items-center gap-2 mb-2">
                            <div class="w-6 h-6 bg-blue-200 rounded-full"></div>
                            <span class="text-xs font-bold">Carlos M.</span>
                            <span class="text-[10px] text-gray-400">2h ago</span>
                        </div>
                        <div class="text-xs text-gray-600">Looking for 2 more people to split Airbnb in Dallas for Quarter Final!</div>
                    </div>
                    <div class="bg-white p-3 rounded-lg shadow-sm">
                        <div class="flex items-center gap-2 mb-2">
                            <div class="w-6 h-6 bg-green-200 rounded-full"></div>
                            <span class="text-xs font-bold">Maria L.</span>
                            <span class="text-[10px] text-gray-400">5h ago</span>
                        </div>
                        <div class="text-xs text-gray-600">Watch party organized! 200+ fans confirmed for Miami match 🎉</div>
                    </div>
                </div>
            </div>
            <h3 class="text-xl font-serif mb-2">Find your travel crew</h3>
            <p class="text-gray-500 text-sm">Connect with fans from your nation, coordinate accommodations, and travel together to matches across North America.</p>
        </div>

        <!-- Card 2 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="bg-green-50 rounded-xl h-64 mb-8 p-4 flex items-center justify-center">
                 <div class="bg-white rounded-xl shadow-lg p-4 w-3/4">
                    <div class="text-xs font-bold mb-3">🚗 Carpool to Stadium</div>
                    <div class="space-y-2 mb-4">
                        <div class="flex items-center justify-between text-xs">
                            <span class="text-gray-500">From:</span>
                            <span class="font-medium">Downtown Miami</span>
                        </div>
                        <div class="flex items-center justify-between text-xs">
                            <span class="text-gray-500">To:</span>
                            <span class="font-medium">Hard Rock Stadium</span>
                        </div>
                        <div class="flex items-center justify-between text-xs">
                            <span class="text-gray-500">Seats:</span>
                            <span class="font-medium text-green-600">3 available</span>
                        </div>
                    </div>
                    <div class="bg-green-500 text-white text-center py-2 rounded-lg text-xs font-bold">Join Carpool</div>
                 </div>
            </div>
            <h3 class="text-xl font-serif mb-2">Organize carpools & transport</h3>
            <p class="text-gray-500 text-sm">Coordinate rides to stadiums, airports, and fan zones. Save money and travel with fellow supporters.</p>
        </div>

        <!-- Card 3 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="bg-orange-50 rounded-xl h-64 mb-8 p-4 flex items-center justify-center">
                <!-- Watch Party Mockup -->
                <div class="bg-white rounded-xl shadow-lg p-4 w-3/4">
                    <div class="text-xs font-bold mb-3">🎉 Watch Party</div>
                    <div class="space-y-2 mb-4">
                        <div class="flex items-center justify-between text-xs">
                            <span class="text-gray-500">Location:</span>
                            <span class="font-medium">Sports Bar Miami</span>
                        </div>
                        <div class="flex items-center justify-between text-xs">
                            <span class="text-gray-500">Time:</span>
                            <span class="font-medium">7:00 PM EST</span>
                        </div>
                        <div class="flex items-center justify-between text-xs">
                            <span class="text-gray-500">Attending:</span>
                            <span class="font-medium text-orange-brand">247 fans</span>
                        </div>
                    </div>
                    <div class="flex gap-2">
                        <div class="w-6 h-6 bg-blue-200 rounded-full"></div>
                        <div class="w-6 h-6 bg-green-200 rounded-full -ml-2"></div>
                        <div class="w-6 h-6 bg-yellow-200 rounded-full -ml-2"></div>
                        <div class="text-xs text-gray-500 ml-1">+244</div>
                    </div>
                </div>
            </div>
            <h3 class="text-xl font-serif mb-2">Find watch parties & rallies</h3>
            <p class="text-gray-500 text-sm">Discover where your nation's fans are gathering. Join massive watch parties and pre-match rallies in every host city.</p>
        </div>

        <!-- Card 4 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="bg-purple-50 rounded-xl h-64 mb-8 p-4 flex items-center justify-center">
                <!-- Group Chat Mockup -->
                <div class="w-full max-w-sm space-y-3">
                    <div class="flex gap-2">
                        <div class="w-8 h-8 bg-blue-200 rounded-full flex items-center justify-center text-xs">🇦🇷</div>
                        <div class="bg-white p-3 rounded-2xl rounded-tl-none shadow-sm text-xs text-gray-600 w-2/3">
                            Anyone want to split a rental car for the Dallas match?
                        </div>
                    </div>
                    <div class="flex gap-2 flex-row-reverse">
                        <div class="w-8 h-8 bg-green-200 rounded-full flex items-center justify-center text-xs">🇦🇷</div>
                        <div class="bg-orange-brand/10 text-gray-700 p-3 rounded-2xl rounded-tr-none shadow-sm text-xs w-2/3">
                            I'm in! Let's coordinate.
                        </div>
                    </div>
                    <div class="flex gap-2">
                        <div class="w-8 h-8 bg-yellow-200 rounded-full flex items-center justify-center text-xs">🇦🇷</div>
                        <div class="bg-white p-3 rounded-2xl rounded-tl-none shadow-sm text-xs text-gray-600 w-2/3">
                            Count me in too! 🚗
                        </div>
                    </div>
                </div>
            </div>
            <h3 class="text-xl font-serif mb-2">Connect with verified fans</h3>
            <p class="text-gray-500 text-sm">Chat directly with fellow supporters from your nation. Coordinate plans, share tips, and build your travel crew in a trusted community.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Early Access CTA -->
  <section class="py-24 bg-cream relative overflow-hidden">
    <!-- Floating Football Icons Background -->
    <div class="absolute inset-0 opacity-5 pointer-events-none">
        <div class="absolute top-10 left-10 text-4xl transform rotate-12">⚽</div>
        <div class="absolute top-20 right-20 text-4xl transform -rotate-6">🏆</div>
        <div class="absolute bottom-20 left-1/3 text-4xl transform rotate-45">⚽</div>
        <div class="absolute bottom-10 right-1/4 text-4xl transform -rotate-12">🏆</div>
    </div>

    <div class="max-w-4xl mx-auto px-4 text-center relative z-10">
        <div class="inline-block bg-orange-brand/10 text-orange-brand px-4 py-1 rounded-full text-xs font-bold mb-6">
            World Cup 2026 • June-July
        </div>
        <h2 class="text-4xl md:text-6xl font-serif mb-4">Join 10,000+ fans <br /> on the waitlist</h2>
        <p class="text-gray-500 mb-10">Be first to access the simulator and connect with your nation's community</p>
        
        <div class="flex justify-center gap-4">
            <Button href="#" type="primary">Join Waitlist &rarr;</Button>
            <Button href="#" type="white">Learn More</Button>
        </div>
    </div>
  </section>

  <!-- Value Proposition Section -->
  <section id="analytics" class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16">
        Save thousands while <br /> experiencing it all
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <!-- Left Large Card -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 md:row-span-2 flex flex-col">
            <div class="mb-8">
                <h3 class="text-xl font-serif mb-2">The cost of going solo</h3>
                <p class="text-gray-500 text-sm">Following your team through the World Cup without coordination means paying premium prices and missing incredible moments.</p>
            </div>
            <div class="flex-1 bg-red-50 rounded-2xl relative overflow-hidden min-h-[300px] p-6">
                <div class="space-y-4">
                    <div class="bg-white p-4 rounded-lg shadow-sm">
                        <div class="flex justify-between items-center mb-2">
                            <span class="text-sm font-medium text-gray-700">Hotels (Solo)</span>
                            <span class="text-lg font-bold text-red-600">$8,000</span>
                        </div>
                        <div class="text-xs text-gray-500">7 nights × $250/night × 4-5 cities</div>
                    </div>
                    <div class="bg-white p-4 rounded-lg shadow-sm">
                        <div class="flex justify-between items-center mb-2">
                            <span class="text-sm font-medium text-gray-700">Transport</span>
                            <span class="text-lg font-bold text-red-600">$2,000</span>
                        </div>
                        <div class="text-xs text-gray-500">Flights, rentals, gas between cities</div>
                    </div>
                    <div class="bg-white p-4 rounded-lg shadow-sm">
                        <div class="flex justify-between items-center mb-2">
                            <span class="text-sm font-medium text-gray-700">Missed Experiences</span>
                            <span class="text-lg font-bold text-red-600">Priceless</span>
                        </div>
                        <div class="text-xs text-gray-500">100+ fan moments you'll never know about</div>
                    </div>
                </div>
                <div class="absolute bottom-6 left-6 right-6">
                    <div class="bg-dark text-white p-4 rounded-lg text-center">
                        <div class="text-xs text-gray-300 mb-1">Total Solo Cost</div>
                        <div class="text-3xl font-bold">$10,000+</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Right Top Card -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="flex justify-between items-start mb-4">
                <div>
                     <h3 class="text-xl font-serif mb-2">With WC26 coordination</h3>
                     <p class="text-gray-500 text-sm">Split costs with your nation's community and save thousands while experiencing everything together.</p>
                </div>
                <span class="bg-green-100 text-green-700 px-2 py-1 rounded text-xs font-bold">Save 60%+</span>
            </div>
            <div class="bg-green-50 rounded-xl p-4">
                <div class="space-y-3">
                    <div class="flex justify-between items-center text-sm">
                        <span class="text-gray-600">Shared Airbnbs</span>
                        <span class="font-bold text-green-600">$2,400</span>
                    </div>
                    <div class="flex justify-between items-center text-sm">
                        <span class="text-gray-600">Carpools</span>
                        <span class="font-bold text-green-600">$600</span>
                    </div>
                    <div class="flex justify-between items-center text-sm">
                        <span class="text-gray-600">Group Activities</span>
                        <span class="font-bold text-green-600">$800</span>
                    </div>
                    <div class="border-t border-green-200 pt-3 flex justify-between items-center">
                        <span class="font-bold text-gray-700">Total Cost</span>
                        <span class="text-2xl font-bold text-green-600">$3,800</span>
                    </div>
                </div>
            </div>
        </div>

        <!-- Right Bottom Card (Savings Highlight) -->
        <div class="bg-gradient-to-br from-green-500 to-green-600 rounded-3xl p-8 shadow-sm flex flex-col justify-center items-center text-white text-center">
            <div class="text-6xl font-serif font-bold mb-2">$6,200</div>
            <div class="text-lg font-medium mb-4">Average savings per fan</div>
            <div class="flex items-center gap-2 text-sm opacity-90">
                <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                <span>Plus 100+ unforgettable moments</span>
            </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Fan Stories Grid -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16 max-w-2xl mx-auto">
        Built by fans who lived the problem
      </h2>

      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-4">
         <!-- Row 1 -->
         <div class="aspect-square bg-gradient-to-br from-blue-400 to-blue-600 rounded-2xl relative overflow-hidden group flex items-center justify-center">
            <div class="text-6xl">🇦🇷</div>
            <div class="absolute bottom-4 left-4 text-white font-bold">Argentina</div>
         </div>
         <div class="aspect-square bg-white rounded-2xl flex items-center justify-center border border-gray-100 p-6">
            <div class="text-center">
                <div class="text-3xl mb-2">⚽</div>
                <div class="text-sm font-bold">10,000+</div>
                <div class="text-xs text-gray-500">Possible Paths</div>
            </div>
         </div>
         <div class="col-span-2 bg-[#FFF9C4] rounded-2xl p-8 flex flex-col justify-between">
            <div class="text-4xl font-serif text-yellow-600">"</div>
            <p class="text-lg font-serif leading-relaxed">Qatar 2022 was incredible but chaotic. I missed so many fan moments because we had no way to coordinate. WC26 changes everything.</p>
            <div class="flex justify-between items-end">
                <div class="text-xs">
                    <div class="font-bold">Karn S.</div>
                    <div class="text-gray-500">Founder, WC26</div>
                </div>
                <div class="text-xl">🏆</div>
            </div>
         </div>

         <!-- Row 2 -->
         <div class="col-span-2 bg-gradient-to-br from-green-400 to-yellow-400 rounded-2xl flex items-center justify-center p-8">
            <div class="text-center text-white">
                <div class="text-5xl mb-2">🇧🇷</div>
                <div class="text-2xl font-bold">Brazil</div>
            </div>
         </div>
         <div class="aspect-square bg-gradient-to-br from-red-400 to-blue-400 rounded-2xl relative overflow-hidden group flex items-center justify-center">
             <div class="text-6xl">🇺🇸</div>
             <div class="absolute bottom-4 left-4 text-white font-bold">USA</div>
         </div>
         <div class="aspect-square bg-gradient-to-br from-white to-red-400 rounded-2xl relative overflow-hidden group flex items-center justify-center">
             <div class="text-6xl">🏴󠁧󠁢󠁥󠁮󠁧󠁿</div>
             <div class="absolute bottom-4 left-4 text-white font-bold">England</div>
         </div>

         <!-- Row 3 -->
         <div class="col-span-2 bg-[#E6F0FF] rounded-2xl p-8 flex flex-col justify-between">
            <div class="text-4xl font-serif text-blue-600">"</div>
            <p class="text-lg font-serif leading-relaxed">The simulator lets me plan every possible scenario. Now I know exactly which cities to book and which matches to attend.</p>
            <div class="flex justify-between items-end">
                <div class="text-xs">
                    <div class="font-bold">Early User</div>
                    <div class="text-gray-500">Beta Tester</div>
                </div>
                <div class="text-xl">🎯</div>
            </div>
         </div>
         <div class="col-span-2 bg-white rounded-2xl flex items-center justify-center border border-gray-100 p-8">
             <div class="text-center">
                <div class="text-4xl font-serif font-bold text-dark mb-2">48 Teams</div>
                <div class="text-sm text-gray-500">16 Cities • 104 Matches</div>
             </div>
         </div>
         
         <!-- Row 4 -->
         <div class="aspect-square bg-gradient-to-br from-green-500 to-red-500 rounded-2xl relative overflow-hidden group flex items-center justify-center">
             <div class="text-6xl">🇲🇽</div>
             <div class="absolute bottom-4 left-4 text-white font-bold">Mexico</div>
         </div>
         <div class="aspect-square bg-gradient-to-br from-blue-500 to-red-500 rounded-2xl relative overflow-hidden group flex items-center justify-center">
             <div class="text-6xl">🇫🇷</div>
             <div class="absolute bottom-4 left-4 text-white font-bold">France</div>
         </div>
         <div class="col-span-2 bg-gradient-to-br from-orange-brand/20 to-orange-brand/10 rounded-2xl flex items-center justify-center p-8 border-2 border-orange-brand">
             <div class="text-center">
                <div class="text-3xl font-serif font-bold text-dark mb-2">Join Your Nation</div>
                <div class="text-sm text-gray-600">Connect with thousands of fans</div>
             </div>
         </div>
      </div>
    </div>
  </section>

  <!-- Primary CTA Section -->
  <section class="bg-orange-brand py-24 relative overflow-hidden">
    <div class="max-w-4xl mx-auto px-4 text-center relative z-10">
        <h2 class="text-4xl md:text-6xl font-serif mb-8 text-dark">Your World Cup journey <br /> starts now</h2>
        
        <div class="flex flex-col md:flex-row justify-center gap-6 mb-10 text-sm font-medium text-dark/80">
            <div class="flex items-center gap-2">
                <div class="bg-dark text-white rounded-full p-0.5"><svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg></div>
                Simulate 10,000+ tournament paths
            </div>
            <div class="flex items-center gap-2">
                <div class="bg-dark text-white rounded-full p-0.5"><svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg></div>
                Save $6,200+ through coordination
            </div>
            <div class="flex items-center gap-2">
                <div class="bg-dark text-white rounded-full p-0.5"><svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg></div>
                Never miss a moment
            </div>
        </div>

        <div class="flex justify-center gap-4">
            <Button href="#" type="primary">Join Waitlist &rarr;</Button>
            <Button href="#" type="white">Explore Simulator</Button>
        </div>
    </div>

    <!-- Bottom Illustration (Football Pattern) -->
    <div class="absolute bottom-0 left-0 right-0 h-32 opacity-10 pointer-events-none flex items-end justify-center overflow-hidden">
        <div class="flex gap-8">
            <div class="text-4xl">⚽</div>
            <div class="text-4xl">🏆</div>
            <div class="text-4xl">⚽</div>
            <div class="text-4xl">🏆</div>
            <div class="text-4xl">⚽</div>
            <div class="text-4xl">🏆</div>
            <div class="text-4xl">⚽</div>
        </div>
    </div>
  </section>

  <!-- How It Works -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16">How It Works</h2>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <!-- Step 1 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="w-12 h-12 bg-orange-brand/10 rounded-full flex items-center justify-center text-orange-brand font-bold text-xl mb-6">1</div>
            <h3 class="text-xl font-serif mb-3">Choose Your Nation</h3>
            <p class="text-gray-600 text-sm mb-6">Join your nation's community and connect with thousands of fans planning their World Cup journey.</p>
            <div class="bg-gray-50 rounded-xl p-4 text-center">
                <div class="text-3xl mb-2">🇦🇷 🇧🇷 🇺🇸</div>
                <div class="text-xs text-gray-500">48 nations available</div>
            </div>
        </div>

        <!-- Step 2 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="w-12 h-12 bg-orange-brand/10 rounded-full flex items-center justify-center text-orange-brand font-bold text-xl mb-6">2</div>
            <h3 class="text-xl font-serif mb-3">Simulate & Plan</h3>
            <p class="text-gray-600 text-sm mb-6">Explore all possible tournament paths. Plan which cities to book, which tickets to buy, before knockout rounds are set.</p>
            <div class="bg-gray-50 rounded-xl p-4">
                <div class="flex items-center justify-between text-xs mb-2">
                    <span class="text-gray-500">Possible Paths</span>
                    <span class="font-bold">10,000+</span>
                </div>
                <div class="flex items-center justify-between text-xs">
                    <span class="text-gray-500">Cities to Visit</span>
                    <span class="font-bold">3-7</span>
                </div>
            </div>
        </div>

        <!-- Step 3 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="w-12 h-12 bg-orange-brand/10 rounded-full flex items-center justify-center text-orange-brand font-bold text-xl mb-6">3</div>
            <h3 class="text-xl font-serif mb-3">Coordinate & Save</h3>
            <p class="text-gray-600 text-sm mb-6">Split Airbnbs, organize carpools, find watch parties. Save thousands while experiencing every moment together.</p>
            <div class="bg-green-50 rounded-xl p-4">
                <div class="flex items-center justify-between mb-2">
                    <span class="text-xs text-gray-600">Average Savings</span>
                    <span class="text-2xl font-bold text-green-600">$6,200</span>
                </div>
                <div class="text-[10px] text-gray-500 text-center">Per fan through coordination</div>
            </div>
        </div>
      </div>
    </div>
  </section>

  <!-- FAQ -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif mb-16">Frequently Asked Questions</h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-x-12 gap-y-6">
        {#each [
            "What is WC26?",
            "How does the tournament simulator work?",
            "What are nation-based communities?",
            "How much can I really save?",
            "Is WC26 only for World Cup 2026?",
            "How do I join my nation's community?",
            "Can I coordinate with fans from other nations?",
            "When does WC26 launch?"
        ] as question}
            <div class="border-b border-gray-200 py-4 flex justify-between items-center group cursor-pointer">
                <span class="font-medium text-lg group-hover:text-orange-brand transition-colors">{question}</span>
                <div class="w-6 h-6 rounded-full bg-dark text-white flex items-center justify-center text-sm group-hover:bg-orange-brand transition-colors">+</div>
            </div>
        {/each}
      </div>
    </div>
  </section>

  <Footer />
</div>

<style>
  /* Custom Scroll Animation */
  @keyframes scroll {
    0% { transform: translateX(0); }
    100% { transform: translateX(-50%); }
  }
  .animate-scroll {
    animation: scroll 20s linear infinite;
  }
  
  @keyframes spin-slow {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
  }
  .animate-spin-slow {
    animation: spin-slow 20s linear infinite;
  }
</style>

