
<h1 align="center">Demo</h1>

## About The Project

<p>Creation of a REST API allowing to handle products</p>
<p>The project contains:</p>
<ul>
  <li>a link to the API documentation</li>
  <li>a endpoint to connection</li>
  <li>endpoints to view products</li>
  <li>endpoints to manage users</li>
   <li>CRUD View</li>
</ul>

<p align="right">(<a href="#top">back to top</a>)</p>

## Built With

This section list the main frameworks/libraries used to start your project.
<ul>
  <li><a href="https://symfony.com/doc/5.4/index.html" target="_blank">Symfony 5.4.7</a></li>
  <li><a href="https://api-platform.com/" target="_blank">API Platform</a></li>
  <li><a href="https://jwt.io/" target="_blank">JWT</a></li>
  <li><a href="https://getbootstrap.com/" target="_blank">Bootstrap</a></li>
  <li><a href="https://jquery.com" target="_blank">JQuery</a></li>
  <li><a href="https://www.php.net/" target="_blank">PHP</a></li>
  <li><a href="https://www.mysql.com/fr/">MySQL</a></li>
  <li><a href="https://twig.symfony.com/" target="_blank">Twig</a></li>
  <li><a href="https://getcomposer.org/" target="_blank">Composer</a></li>
</ul>

<p align="right">(<a href="#top">back to top</a>)</p>

## Prerequisites

This is the list of things you need to use the software.
   ```sh
      - PHP: >=7.4
      - MySQL
      - Composer (https://getcomposer.org/)
      - OpenSSL (https://www.openssl.org/)
   ```

## Getting Started

To get a local copy up and running follow these simple example steps :

1.&nbsp;Clone the repo

2.&nbsp;Install composer packages and npm packages
   ```sh
   composer install
   ```
   ```sh
   npm install
   ```
3.&nbsp;You customize variables of file **.env** as needed to run the environment.
   ```sh
   DATABASE_URL="mysql://db_user:db_password@127.0.0.1:3306/db_name?serverVersion=5.7&charset=utf8mb4"
   JWT_PASSPHRASE=EnterYourPassPhraseHere # required for token creation
   ```
4.&nbsp;Create database
   ```sh
   php bin/console doctrine:database:create
   ```
   ```sh
   php bin/console doctrine:migrations:migrate
   ```
5.&nbsp;Load fixtures
   ```sh
   php bin/console doctrine:fixtures:load
   ```
6.&nbsp;Generate the SSL keys
   ```sh
   php bin/console lexik:jwt:generate-keypair
   ```
7.&nbsp;Run project
   ```sh
   php -S localhost:8000 -t public/
   ```  
8.&nbsp;Documentation link : http://localhost:8000

9.&nbsp;Log in with an account :

   Administrator account
   ```sh
   -Username : admin@admin.com
   -Password : password
   ```

<p align="right">(<a href="#top">back to top</a>)</p>

