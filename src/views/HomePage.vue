<script setup>
const spin = () => alert('Hello')
</script>

<template>
  <main
    class="min-h-screen bg-[radial-gradient(circle_at_15%_20%,#334155,transparent_40%),radial-gradient(circle_at_85%_0%,#0f766e,transparent_28%),linear-gradient(160deg,#020617,#0f172a,#111827)] px-4 py-8 text-slate-100 sm:px-6 lg:px-8"
  >
    <div class="mx-auto max-w-7xl">
      <header class="mb-8">
        <p class="text-xs font-semibold tracking-[0.3em] text-blue-500 uppercase">Project #4</p>
        <h1 class="mt-2 text-4xl font-black text-white sm:text-5xl">Anime Roulette Machine</h1>
        <p class="mt-2 max-w-2xl text-sm text-slate-300 sm:text-base">
          Spin the reel, request a random anime from Jinkan with VueUse useFech, and learn how REST
          APIs signal rate limiting with HTTP 429
        </p>
      </header>

      <div class="grid gap-6 lg:grid-cols-[1.2fr_0.8fr]">
        <section class="space-y-5">
          <div
            class="boarder border-slate700/70 shadow-2xlshadow-slate-950/30 rounded-3xl bg-slate-900/60 p-5 backdrop-blur-sm"
          >
            <div class="flex flex-col sm:flex-row sm:items-center sm:justify-between">
              <div>
                <h2 class="text-xl font-bold text-white">Roulette</h2>
                <p class="text-sm text-slate-300">
                  Pull the lever for your next raondom anime recommendation.
                </p>
              </div>
              <button
                type="button"
                class="cursor-pointer rounded-full border-blue-400/70 bg-cyan-300/20 px-6 py-3 text-base font-black tracking-wide text-cyan-100 hover:bg-blue-400/30"
                @click="spin"
              >
                Spin
              </button>
            </div>
          </div>
        </section>
      </div>
    </div>
  </main>
</template>
