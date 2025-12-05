# Sistema Laravel 12 com autenticação por login

> Sistema Laravel 12 com pacote de autenticação por login, registro de usuário, perfil e verificação em 2 etapas 2FA já instalados e configurados.

---

## 🧰 Tecnologias Utilizadas

-   **PHP 8.3+**
-   **Laravel 12**
-   **Jetstream + Livewire**
-   **MySQL 8**
-   **Pacote de tradução pt_BR**

---

## ⚙️ Instalação e Configuração (Ambiente de Desenvolvimento)

### 🔹 Pré-requisitos

Antes de começar, verifique se possui os seguintes itens instalados:

-   [Laragon](https://laragon.org) (ou outro ambiente compatível com PHP 8.3+, MySQL, Composer e Node.js + NPM)

---

### 🔹 Passos para instalação

1. **Clonar o repositório**

    ```bash
    git clone https://github.com/renatotg10/laravel12_jetstream_livewire.git
    cd laravel12_jetstream_livewire
    ```

2. **Instalar dependências do Laravel**

    ```bash
    composer install
    ```

3. **Instalar dependências do frontend**

    ```bash
    npm install
    ```

4. **Gerar o arquivo `.env`**

    ```bash
    cp .env.example .env
    ```

5. **Configurar das variáveis de ambiente no arquivo `.env`**

   No arquivo `.env`, ajuste as variáveis de ambiente para uso do idioma pt_BR, banco de dados MySQL e uso do Mailpit no Laragon, que é uma ferramenta usada como servidor de e-mail fake/local para desenvolvimento.

    ```env
    APP_NAME=Laravel
    APP_URL=http://localhost:8000

    APP_LOCALE=pt_BR
    APP_FALLBACK_LOCALE=pt_BR
    APP_FAKER_LOCALE=pt_BR

    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=laravel
    DB_USERNAME=root
    DB_PASSWORD=

    MAIL_MAILER=smtp
    MAIL_HOST=127.0.0.1
    MAIL_PORT=1025
    MAIL_USERNAME=null
    MAIL_PASSWORD=null
    MAIL_ENCRYPTION=null
    MAIL_FROM_ADDRESS="noreply@meusistema.com"
    MAIL_FROM_NAME="${APP_NAME}"
    ```

_Observação:_ Se estiver executando a partir do servidor Apache do Laragon, ajuste a variável de ambiente `APP_URL` no arquivo `.env` para `APP_URL=http://laravel12_jetstream_livewire.test`. Lembre-se sempre de atualizar nessa variável de ambiente a URL que acessa ao sistema.

6. **Gerar a chave da aplicação**

    ```bash
    php artisan key:generate
    ```

7. **Compilar os assets**

    ```bash
    npm run build
    ```

8. **Iniciar o servidor local**

    ```bash
    php artisan serve
    ```

    O sistema estará disponível em:
    👉 [http://localhost:8000](http://localhost:8000)

---

## 🌐 Tradução para Português

**O projeto já inclui o pacote de tradução em português-BR**.

Caso precise atualizar ou reinstalar (**somente se precisar atualizar ou reinstalar**), execute:

```bash
composer require laravel-lang/lang --dev
php artisan lang:publish
```

---

## 📄 Licença

Este projeto está licenciado sob a Licença GPL-3.0. Consulte o arquivo [LICENSE](LICENSE) para detalhes.

---

## 🧭 Contato

👤 _Renato Gomes_
📧 `renatotg10@gmail.com`


