# 🧑‍💻 Portfoleo

<div align="center">

<img src="./.gitassets/capa.png" width="350px">

<div data-badges>
  <img src="https://img.shields.io/badge/next.js-%23000000.svg?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" />
    <img src="https://img.shields.io/badge/nestjs-%23E0234E.svg?style=for-the-badge&logo=nestjs&logoColor=white" alt="NestJS" />
    <img src="https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
    <img src="https://img.shields.io/badge/prisma-%232D3748.svg?style=for-the-badge&logo=prisma&logoColor=white" alt="Prisma" />
    <img src="https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="TailwindCSS" />
    <img src="https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB" alt="React" />
    <img src="https://img.shields.io/badge/n8n-%2300C4B4.svg?style=for-the-badge&logo=n8n&logoColor=white" alt="n8n" />
    <img src="https://img.shields.io/badge/supabase-%233ECF8E.svg?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase" />
</div>

</div>
<br/>

*O Portfoleo é uma aplicação full stack que integra tecnologias populares do mercado para criar uma vitrine digital das habilidades e projetos de um desenvolvedor. Esta plataforma vai além da simples exibição de trabalhos anteriores, funcionando como uma demonstração prática das capacidades técnicas do profissional, evidenciando seu domínio em desenvolvimento web moderno.*

*Além de apresentar os projetos do desenvolvedor, a aplicação incorpora agentes de IA inteligentes que têm acesso completo ao currículo, repositórios do GitHub e histórico do profissional. Essa integração permite que recrutadores e potenciais clientes explorem, através de interações em tempo real via chat, aspectos específicos das competências técnicas do desenvolvedor. Os chats com os agentes oferecem insights valiosos, permitindo que visitantes façam perguntas e recebam informações detalhadas sobre as habilidades e experiências do profissional, tornando o processo de avaliação mais dinâmico e informativo.*

## 🖥️ Como rodar este projeto 🖥️

### Requisitos:

-   **Node.js instalado**

### Execução:

1. **Clone este repositório:**

    ```sh
    git clone https://github.com/portfolio-projetos-dev/portfoleo.git
    ```

2. **Acesse o diretório do projeto:**

    ```sh
    cd portfoleo
    ```

3. *Acesse sua conta no* **[Supabase](https://supabase.com)** *ou crie uma nova conta.*

4. *Navegue até o projeto no* **Supabase** *e clique no botão **`connect`**.*
   
5. *Clique em selecionar* **ORM** *e selecione o* **ORM Prisma**.
   
6. *Copie as variáveis de ambiente listadas, crie um arquivo* `.env` *na pasta backend e preencha com as seguintes informações:*
    ```
    DATABASE_URL=
    DIRECT_URL=
    PORT=
    ```
    **Obs: Caso o valor da porta não seja adicionado, a aplicação rodará por padrão na porta 4000**

7. *Crie uma conta no site no* **[n8n](https://n8n.io)**, *e importe o fluxo definido no arquivo assistente-pessoal que está na pasta assets.*

8. *Após importar o fluxo, clique no primeiro nó, acesse* `webhooks url`, *clique em* `Production URL` *e copie o valor dessa URL.*
**Obs: Lembre-se de ativar o workflow no n8n**

9. *Crie um arquivo* `.env` *na pasta web e preencha com as seguintes informações, sendo que a URL da API é a URL do backend e a segunda variável deve ter como valor a URL que extraimos no n8n:*

    ```
    NEXT_PUBLIC_API_URL=
    NEXT_PUBLIC_CHAT_WEBHOOK=
    ```

10. *Instale as dependências dos projetos* `web` *e* `backend` *com o comando* `npm i` *em cada uma das pastas.*

11. *Abra as pastas* `web` *e* `backend` *em dois terminais diferentes e rode o comando* `npm run dev` *em cada um dos terminais para executar o projeto.*

## 🗒️ Features do projeto 🗒️

-   **Exibição de Projetos**
-   **Integração com Agentes de IA via Chat**
-   **Repositórios GitHub Integrados**
-   **Lista de tecnologias destacadas**
-   **Lista de tecnologias dos projetos**
-   **Buscar os projetos por Id com as tecnologias associadas**

![](./.gitassets/2.png)   

## 💎 Links úteis 💎

-   **[Next.js](https://nextjs.org/docs)**
-   **[NestJS](https://docs.nestjs.com/)**
-   **[Prisma](https://www.prisma.io/docs)**
-   **[Supabase](https://supabase.com)**

<svg width="15" height="15" viewBox="0 0 15 15" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M1 2C0.447715 2 0 2.44772 0 3V12C0 12.5523 0.447715 13 1 13H14C14.5523 13 15 12.5523 15 12V3C15 2.44772 14.5523 2 14 2H1ZM1 3L14 3V3.92494C13.9174 3.92486 13.8338 3.94751 13.7589 3.99505L7.5 7.96703L1.24112 3.99505C1.16621 3.94751 1.0826 3.92486 1 3.92494V3ZM1 4.90797V12H14V4.90797L7.74112 8.87995C7.59394 8.97335 7.40606 8.97335 7.25888 8.87995L1 4.90797Z" fill="currentColor" fill-rule="evenodd" clip-rule="evenodd"></path></svg>