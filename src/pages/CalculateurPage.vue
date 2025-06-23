<template>
    <div class="bg-gray-100 dark:bg-gray-900">
        <LP_Header />
        <div class="py-8 px-4 mx-auto max-w-screen-xl lg:py-16 lg:px-6">
            <h1 class="mb-4 text-3xl font-extrabold text-center tracking-tight leading-none text-gray-900 md:text-4xl lg:text-5xl dark:text-white">
            Tajimo 💼📊 • Calculateur de TJM
            </h1>
            <p class="mb-8 text-lg font-normal text-center text-gray-500 lg:text-xl sm:px-16 xl:px-28 dark:text-gray-400">
            Tajimo vous aide à calculer votre TJM idéal en prenant en compte vos charges, votre imposition, vos jours non facturés et vos objectifs de revenus. Simple, rapide et pensé pour les freelances.
            </p>
                    <div class="w-full p-4">
            <div class="grid grid-cols-1 gap-y-4 gap-x-1 auto-rows-auto">
                <Remuneration />
                <FraisFonctionnement />
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <ChargesSociales />
                    <Impositions />
                </div>
                <DecompteJour />
                <EstimationFinale />
            </div>
        </div>
        <LP_Testimonials />
                </div>
        <LP_Footer />
    </div>
</template>

  <script setup>
  import LP_Header from '../components/Landing/LP_Header.vue'
  import Remuneration from '../components/Calculateur/Remuneration.vue'
  import FraisFonctionnement from '../components/Calculateur/FraisFonctionnement.vue'
  import ChargesSociales from '../components/Calculateur/ChargesSociales.vue'
  import Impositions from '../components/Calculateur/Impositions.vue'
  import DecompteJour from '../components/Calculateur/DecompteJour.vue'
  import EstimationFinale from '../components/Calculateur/EstimationFinale.vue'
  import LP_Testimonials from '../components/Landing/LP_Testimonials.vue'
  import LP_Footer from '../components/Landing/LP_Footer.vue'


  import { provide } from 'vue'
  import { useCalculator } from '../composables/useCalculator'

  // On initialise une seule fois l’état du calculateur
  const calculator = useCalculator()

  // On le fournit à toute la hiérarchie
  provide('calculator', calculator)
  </script>