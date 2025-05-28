<template>
  <main class="min-h-screen text-white mt-30 ml-50 w-300">
    <div class="grid grid-cols-2 gap-10">
      <div class="about">
        <p class="text-3xl">Olá! Sou o Igor</p>
        <p class="text-3xl">Tenho 26 anos e atuo como Desenvolvedor.</p>

        <!-- Animação aqui -->
        <p class="text-xl text-teal-400 mt-4 h-8">
          Stacks - <span>{{ displayedText }}</span>
        </p>

        <div class="text-gray-400 text-xl mt-6">
          <ul class="space-y-6">
            <li>
              Venho me aprofundando em desenvolvimento web, construção de APIs, bancos de dados e boas práticas de programação. Estou sempre em busca de evoluir tecnicamente, contribuindo com soluções eficientes e bem estruturadas.
            </li>
            <li>
              Antes disso, atuei por 4 anos como Analista de Dados, onde desenvolvi habilidades sólidas em Power BI, SQL, Excel, Python e R. Nesse período, fui responsável por transformar dados em insights valiosos que impactaram diretamente na tomada de decisões e nos resultados das empresas em que passei.
            </li>
            <li>
              Essa transição representa mais do que uma mudança de carreira, é a continuação do meu desejo de resolver problemas de forma criativa e de impactar positivamente o maior número de pessoas possível por meio da tecnologia.
            </li>
          </ul>
        </div>
      </div>

      <div class="image ml-50">
        <img src="../images/Igor.jpg" alt="Igor" />
      </div>
    </div>
  </main>
</template>

<script setup>
import { ref, onMounted } from 'vue'

const displayedText = ref('')
const words = ['.NET', 'JavaScript','Vue', 'SQL']
let wordIndex = 0
let charIndex = 0
let typing = true

function typeLoop() {
  const currentWord = words[wordIndex]

  if (typing) {
    if (charIndex < currentWord.length) {
      displayedText.value += currentWord[charIndex]
      charIndex++
      setTimeout(typeLoop, 100)
    } else {
      typing = false
      setTimeout(typeLoop, 1500)
    }
  } else {
    if (charIndex > 0) {
      charIndex--
      displayedText.value = currentWord.slice(0, charIndex)
      setTimeout(typeLoop, 50)
    } else {
      typing = true
      wordIndex = (wordIndex + 1) % words.length
      setTimeout(typeLoop, 500)
    }
  }
}

onMounted(() => {
  typeLoop()
})
</script>
