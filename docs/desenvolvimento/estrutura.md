## Pastas e Estrutura

A estrutura do projeto é a seguinte:

```plaintext
CellarCRM/
│
├── app/
│   ├── Console/
│   ├── Exceptions/
│   ├── Http/
│   │   ├── Controllers/
│   │   ├── Middleware/
│   ├── Models/
│   ├── Providers/
│
├── bootstrap/
│
├── config/
│   ├── google-cloud/
│
├── database/
│   ├── factories/
│   ├── migrations/
│   ├── seeders/
│
├── lang/
│   ├── pt/
|
├── public/
│   ├── assets/
│   │   ├── css/
│   │   ├── fonts/
│   │   ├── images/
│   │   ├── js/
│   │   │    ├── pages/
│   │   ├── libs/
│   ├── css/
│   ├── images/
│   ├── js/
│   ├── storage/
│   ├── vendor/
│
├── resources/
│
│   ├── views/
│
├── routes/
│
├── storage/
│   ├── app/
│   │    ├── public/
│   ├── framework/
│   ├── logs/
│
├── tests/
│
├── vendor/
│
├── .env
├── artisan
├── composer.json
├── phpunit.xml
└── server.php
```

*   **app/**: Contém o código-fonte da aplicação, incluindo controllers, models, e outros.
*   **bootstrap/**: Contém os scripts necessários para inicializar o aplicativo.
*   **config/**: Armazena configurações do aplicativo.
*   **database/**: Contém migrations, seeders e factories para gerenciar o banco de dados.
*   **public/**: O diretório acessível publicamente. Arquivos como CSS, JavaScript e imagens devem ser colocados aqui.
*   **resources/**: Contém views, arquivos de tradução e ativos não compilados, como Sass e JavaScript.
*   **routes/**: Define as rotas da aplicação.
*   **storage/**: Armazena arquivos gerados dinamicamente, como logs, caches, e uploads.
*   **tests/**: O diretório para os testes automatizados.
*   **.env**: Arquivo de ambiente, onde você configura as variáveis de ambiente, incluindo detalhes do banco de dados e chaves de aplicativos.
*   **artisan**: O script de linha de comando para interagir com o Laravel.
*   **composer.json**: O arquivo de configuração para o Composer, que gerencia as dependências do projeto.
*   **phpunit.xml**: Configurações para PHPUnit, usado para testes automatizados.
*   **server.php**: O script de servidor embutido.