# To-Do-List


-Aplicação Web, front-end e back end;

-Utilizei o servidor xampp para rodar a aplicação localmente.

-Para rodar em sua máquina basta instalar o XAMPP em sua última versão ou instalar o Apache via VsCode, após isso caso tenha instalado o XAMPP você irá colocar os arquivos dentro de uma pasta chamada to-do-list dentro da pasta htdocs do Xampp, em seguida rode o xampp e ative o servidor Apache e acesse em seu navegador http://localhost/to-do-list/.

-O Arquivo to-do-list.SQL é o banco de dados da aplicação Web, para integrá-lo você irá iniciar o servidor MYSQL do XAMPP e acessar http://localhost/phpmyadmin/, lá você vai em "importar" e logo após "escolher arquivo" em "Ficheiro a importar" e execute.

Pronto.

-Para acessar pelo celular, basta permitir o servidor Apache através do firewall e coloque o IP local IPV4 da máquina onde você está hospedando localmente sua aplicação.

-Caso o navegador recuse a requisição, vá no apache> config> Apache (httpd-xampp.conf) e altere o documento.


    <Directory "C:/xampp/phpMyAdmin">
       AllowOverride AuthConfig
       **Require local**   Altere para   **Require all granted**
       ErrorDocument 403 /error/XAMPP_FORBIDDEN.html.var
   </Directory>```
   
   

[ENGLISH]

-Web application, front-end and back-end;

-I used the xampp server to run the application locally.

-To run on your machine just install XAMPP in its latest version or install Apache via VsCode, after that if you have installed XAMPP you will place the files inside a folder called to-do-list inside the Xampp htdocs folder, then run xampp and activate the Apache server and access in your browser http://localhost/to-do-list/.

-The file to-do-list.SQL is the database of the Web application, to integrate it you will start the XAMPP MYSQL server and access http://localhost/phpmyadmin/, there you will go to "import" and right after "choose file" in "File to import" and execute.

Ready.

-To access by cell phone, simply allow the Apache server through the firewall and place the local IPV4 IP of the machine where you are hosting your application locally.

-If the browser refuses the request, go to apache> config> Apache (httpd-xampp.conf) and change the document.
    
    
    <Directory "C:/xampp/phpMyAdmin">
       AllowOverride AuthConfig
       **Require local**   Replace with   **Require all granted**
       ErrorDocument 403 /error/XAMPP_FORBIDDEN.html.var
   </Directory>```
