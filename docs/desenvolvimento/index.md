## Instalação

### Dependências do Projeto

```html
"require": {
        "php": "^8.1",
        "google/cloud-bigquery": "^1.28",
        "google/recaptcha": "^1.3",
        "guzzlehttp/guzzle": "^7.2",
        "intervention/image": "^2.7",
        "laravel/framework": "^10.10",
        "laravel/sanctum": "^3.3",
        "laravel/tinker": "^2.8",
        "laravel/ui": "^4.2"
    },
    "require-dev": {
        "fakerphp/faker": "^1.9.1",
        "laravel/breeze": "^1.26",
        "laravel/pint": "^1.0",
        "laravel/sail": "^1.18",
        "laravel/telescope": "^4.17",
        "mockery/mockery": "^1.4.4",
        "nunomaduro/collision": "^7.0",
        "phpunit/phpunit": "^10.1",
        "spatie/laravel-ignition": "^2.0"
    }
```

## Processo de Instalação

Instale o GIT em sua máquina. Se tiver dúvidas, siga o passo-a-passo no site [https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Instalando-o-Git](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Instalando-o-Git)

Vá para sua pasta padrão de projetos, se não tiver uma, crie.

Dentro da sua pasta de projetos, abra o terminal e clone o projeto Cellar CRM com o seguinte comando:

Clone o repositório do Git:

```plaintext
git clone https://github.com/cellarvinhostechteam/CellarCRM.git
```

> Como o nosso projeto é **Privado** o Git irá solicitar seus dados de login. Caso não tenha ainda permissões como colaborador(a) do projeto, peça ao seu superior.

Navegue para o diretório do projeto:

```plaintext
cd CellarCRM
```

  
Instale as dependências do Composer:

```plaintext
composer install
```

  
Copie o arquivo de configuração do ambiente:

```plaintext
cp .env.example .env
```

No arquivo .env você precisará inserir as informações do seu banco de dados MySQL:

```plaintext
DB_CONNECTION=mysql
DB_HOST=seu_host
DB_PORT=seu_porta
DB_DATABASE=seu_banco_de_dados
DB_USERNAME=seu_usuario
DB_PASSWORD=sua_senha
```

*   **DB\_CONNECTION**: O tipo de conexão com o banco de dados. No exemplo, está configurado para MySQL, mas você pode ajustar para outros suportados pelo Laravel, como PostgreSQL, SQLite, SQL Server, etc.
*   **DB\_HOST**: O endereço do servidor do banco de dados.
*   **DB\_PORT**: A porta do banco de dados.
*   **DB\_DATABASE**: O nome do banco de dados que você está usando.
*   **DB\_USERNAME**: O nome de usuário do banco de dados.
*   **DB\_PASSWORD**: A senha associada ao nome de usuário do banco de dados.

Gere a chave de aplicação:

```plaintext
php artisan key:generate
```

  
Configure o arquivo .env com as informações do banco de dados e outras configurações necessárias.

Execute as migrações do banco de dados:

```plaintext
php artisan migrate
```

Para executar os seeders no Laravel, após ter realizado as etapas de migração, você pode usar o seguinte comando:

```plaintext
php artisan db:seed
```

  
Link simbolicamente o armazenamento público:

```plaintext
php artisan storage:link
```

  
Inicie o servidor embutido (opcional):

```plaintext
php artisan serve
```

Após este comando você deverá ver algo como o seguinte:

```plaintext
INFO  Server running on [http://127.0.0.1:8000].

Press Ctrl+C to stop the server
```

Caso você queira rodar o projeto em outra porta, rode o seguinte comando:

```plaintext
php artisan serve --port=8080
```

**Pronto!**

Você já está com o projeto CellarCRM rodando localmente em sua máquina