<h1>README - Imagens de Raposa</h1>

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

<h4>Este projeto é uma aplicação web que exibe imagens aleatórias de raposas. Ele utiliza HTML, CSS e JavaScript para criar uma interface interativa onde os usuários podem atualizar a imagem de raposa com um clique de botão.</h4>

<h1>Estrutura do Projeto</h1>
<h4>O projeto é composto por um único arquivo HTML. Aqui está uma visão geral da estrutura:</h4>

<h4>HTML: Define a estrutura básica da página, incluindo uma imagem e um botão.</h4>
<h4>CSS: Estiliza a página para uma melhor apresentação.</h4>
<h4>JavaScript: Faz a chamada à API para obter uma nova imagem de raposa e atualiza a interface.</h4>
<h1>Funcionalidades</h1>
<h4>Exibição de Imagem: A imagem de uma raposa é exibida na página.</h4>
<h4>Atualização de Imagem: Um botão permite ao usuário atualizar a imagem para uma nova raposa aleatória.</h4>
<h4>Carregamento Inicial: Uma imagem é carregada automaticamente ao abrir a página.</h4>
<h1>Como Usar</h1>
<h4>Clone ou baixe o repositório.
Abra o arquivo HTML em um navegador web.
Clique no botão "Atualizar Imagem" para obter uma nova imagem de raposa.</h4>
<h1>Tecnologias Utilizadas</h1>
<h4>HTML5: Para estruturar o conteúdo da página.</h4>
<h4>CSS3: Para estilização e layout responsivo.</h4>
<h4>JavaScript: Para interatividade e manipulação do DOM.</h4>
<h4>API: Utiliza a API Random Fox para obter imagens de raposas.</h4>
<h1>Detalhes do Código</h1>

<h1>HTML:</h1>

O elemento <img> é usado para exibir a imagem da raposa.
O botão chama a função getFoxIMG() quando clicado.

```
<img id="foxImage" src="" alt="Imagem de Raposa">
    <button onclick="getFoxIMG()">Atualizar Imagem</button>
```
<h1>CSS:</h1>

<h4>Estilização do corpo da página para centralizar o conteúdo.
Estilos aplicados à imagem e ao botão para melhorar a aparência.</h4>

```
<style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
        }
        img {
            max-width: 100%;
            height: auto;
            border: 2px solid #ccc;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        button {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 16px;
            color: #fff;
            background-color: #007BFF;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
```
<h1>JavaScript:</h1>

<h4>A função getFoxIMG() faz uma chamada à API e atualiza a imagem.
O método fetch() é utilizado para obter os dados da API.
Um tratamento de erro simples é implementado para capturar problemas na requisição.</h4>

```
 <script>
        function getFoxIMG() {
            fetch(https://randomfox.ca/floof/)
                .then(response => response.json())
                .then(data => {
                    document.getElementById('foxImage').src = data.image;
                })
                .catch(error => console.error('Erro:', error));
        }

        // Carregar uma imagem ao iniciar
        getFoxIMG();
    </script>
```


<h1>Aproveite as adoráveis imagens de raposas! 🦊</h1>

<h2 id="autores"> Autores </h2>

<h3>Naomi Arakaki</h3>



[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white&link=https://www.linkedin.com/in/naomi-suguimoto-57436b290/)](https://www.linkedin.com/in/naomi-suguimoto-57436b290)

[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white&link=mailto:arakakinaomi228@gmail.com)](mailto:arakakinaomi228@gmail.com)


<h3>Gabriel Aboboreira</h3>


[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white&link=https://www.linkedin.com/in/gabriel-aboboreira/)](https://www.linkedin.com/in/gabriel-aboboreira/)

[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white&link=mailto:masterkillbr007@gmail.com)](mailto:masterkillbr007@gmail.com)


<h3>Ana Julia Blande</h3>

[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white&link=https://www.linkedin.com/in/gabriel-aboboreira/)](https://www.linkedin.com/in/gabriel-aboboreira/)

[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white&link=mailto:anajblande04@gmail.com)](mailto:anajblande04@gmail.com)


