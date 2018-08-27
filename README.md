# Instala-o-Laravel

MANUAL DE INSTALAÇÃO DO LARAVEL NO "WINDOWS"

1° Instale o APACHE na sua máquina;

	# (https://www.apachefriends.org/pt_br/index.html)

	# Caso não esteja conseguindo instalar o xampp veja este tutorial: (https://www.youtube.com/watch?v=RrzmxeQOcYg)

2° Confira se o Composer está instalado na sua máquina;
	
	# (Abra o Prompt de Comando do Windows e digite: composer)

3° Caso, se ja tenha instalado vá no painel de controle e desinstale da sua máquina;

4° Instale o Composer;
	
	# (https://getcomposer.org/download/)  ---> Baixe o "Composer-Setup.exe"

5° Na instalação do composer direcione para a pasta do PHP que está dentro da pasta XAMPP.
	
	# Exemplo:(C:\xampp\php\php.exe)

6° Crie um projeto laravel

	# Abra o Prompt de comando e digite esses comandos:

--------------------------------------------------------------------------------------------

	   cd\
	   cd xampp\htdocs
	   composer create-project --prefer-dist laravel/laravel pastaDoMeuProjetoLaravel
	
--------------------------------------------------------------------------------------------

	# Observação: No "pastaDoMeuProjetoLaravel" apague e coloque o nome de sua escolha para o seu projeto laravel
	
	
	 
7° Geralmente no Windows ele não gera o 'key' => env('APP_KEY'),

	# Vá na pasta do seu projeto laravel, entre na pasta /config e abra o arquivo app.php 

	# Confira no app.php se ele está assim: 'key' => env('APP_KEY')

	# Caso ele esteja sem o Key. Vá no Prompt de comando do windows e digite:

--------------------------------------------------------------------------------------------

	   cd\
	   cd xampp\htdocs\
	   cd pastaDoMeuProjetoLaravel
	   php artisan key:generate

	# observação: No "pastaDoMeuProjetoLaravel" apague e coloque o nome da pasta que está SEU PROJETO LARAVEL

--------------------------------------------------------------------------------------------
	# Ainda no Prompt de comando do Windows Onde está o nome:

	    Application key [base64:xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx=] set successfully.

	# Copie toda a chave que começa depois do base64: e acaba no =

	# Exemplo copiando a chave ácima: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

8° Cole a chave que gerou no Prompt de comando do Windows, no arquivo app.php 

	# Vá na pasta do seu projeto laravel, entre na pasta /config e abra o app.php  

	# Cole a chave como no exemplo abaixo: 

	   'key' => env('APP_KEY','xxxxxxxxxxxxxxxxxxxxxxxxxxxxx'),

9° Abra o chrome e veja se está funcionando o laravel;

	Digite na url:

	localhost/pastaDoMeuProjetoLaravel/public


--------------------------------------------------------------------------------------------------------------------------


SUCESSOOOO!!!!!

Produzido por: Rodrigo Queiroz
