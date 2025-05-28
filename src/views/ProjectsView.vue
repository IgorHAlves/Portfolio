<template>
<main class="mt-30 justify-items-center">

    <h1 class="text-white text-center mt-20 text-6xl">Projetos</h1>

    <div class="py-20 flex min-h-screen flex-col items-center text-white">

        <div class="flex items-center justify-center px-6 space-x-10 text-left max-w-6xl mb-12 mr-80">
            <img class="w-[400px] h-auto rounded-xl shadow-lg shadow-gray-100/20" src="../images/SwaggerMercearia.png" alt="">
            <p class="text-xl text-gray-400">Este projeto é uma API desenvolvida para gerenciar uma mercearia fictícia, permitindo operações CRUD (Create, Read, Update, Delete) para Clientes, Produtos e Pedidos. A API utiliza o SQL Server como banco de dados, configurado no Docker para facilitar a execução e manutenção do ambiente.</p>
        </div>

        <div class="flex items-center justify-center px-6 space-x-10 text-left max-w-6xl ml-80">
            <p class="text-xl text-gray-400">Este projeto FullStack no modelo MVC, onde no Back-end foi desenvolvido um banco de dados Postgres e uma API .NET para intermediar a comunicação entre o Front-end e o banco. A API permite operações CRUD (Create, Read, Update, Delete) no banco criado e também se comunica com a api Randon User Generator (https://randomuser.me) para gerar Users de forma aleatória e fazer a persistência dos mesmos no banco de dados. Ressalto que no projeto também foi utilizado o Docker para facilitar a execução do Banco de Dados.

            </p>
            <div class="w-1000">
                <img class="mb-2 w-[500px] h-auto rounded-xl shadow-lg shadow-gray-100/20" src="../images/RandomUserGeneratorFrontend.png" alt="">
                <img class="w-[500px] h-auto rounded-xl shadow-lg shadow-gray-100/20" src="../images/RandomUserGeneratorBackend.png" alt="">

            </div>
        </div>
        
    <div class="flex items-center justify-center px-6 space-x-10 text-left max-w-6xl mb-12 mr-80 mt-15">
        <img class="w-[400px] h-auto rounded-xl shadow-lg shadow-gray-100/20" src="../images/UniMovie.png" alt="">
        <p class="text-xl text-gray-400">Projeto desenvolvido para estudo e aprofundamento nos conhecimentos de HTML, CSS, Boostrap e JavaScript, onde foi feita uma navbar e o consumo de uma API, criando cards dinamicos de acordo com o retorno da API e disponibilizando a opção de filtrar os elementos que aparecem na tela.</p>
    </div>


    </div>
</main>
</template>
