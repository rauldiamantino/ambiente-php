## Configurar Ambiente de Desenvolvimento PHP [Windows]

1. Instalar o Visual C++;
2. Faça o <a href="https://windows.php.net/download#php-8.2">Download do PHP</a> conforme versão do Windows;
3. Criar uma pasta chamada `php` em `C:` descompactar os arquivos do PHP nela;
4. Localizar o arquivo `php.ini-development` e remover o termo `-development`, o arquivo deverá ficar como nome `php.ini`. Assim podemos utlizar o php no localhost;
5. Adicionar o PHP nas variáveis do sistema, dessa forma ele poderá ser executado de qualquer local da máquina, independente se está no `C:` ou não;
	1. `Control Panel` > `System and Security` > `See the name of this computer` > `Advanced system setting` > `Environment Variables` > `Path` > `New` > `C:\php`;
	2. abrir o cmd do windows e digitar `php --version`. Deve retornar a versão do php;
	3. executar o notepad como administrador, clicar em `File` > `Open` > `C:\Windows\System32\drivers\etc` > `todas as extensões` > `hosts.old`;
	4. remover o comentário # da linha "127.0.0.1 localhost". Se não tiver essa linha, basta adicioná-la;
6. Para rodar o servidor digite no terminal: `php -S localhost:8000`;

Fonte: https://www.youtube.com/watch?v=HzIXZVctwI8
