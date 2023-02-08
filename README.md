## Configurar Ambiente de Desenvolvimento PHP [Windows]

1. Instale o <a href="https://learn.microsoft.com/pt-br/cpp/windows/latest-supported-vc-redist?view=msvc-170">Visual C++</a>;
2. Faça o <a href="https://windows.php.net/download#php-8.2">Download do PHP</a> conforme versão do Windows;
3. Crie uma pasta chamada `php` em `C:` e descompacte os arquivos do PHP nela;
4. Localize o arquivo `php.ini-development` e remova o termo `-development`, o arquivo deverá ficar como nome `php.ini`. Assim podemos utlizar o php no localhost;
5. Adicione o PHP nas variáveis do sistema, dessa forma ele poderá ser executado de qualquer local da máquina, independente se está no `C:` ou não;
	1. Vá em `Control Panel` > `System and Security` > `See the name of this computer` > `Advanced system setting` > `Environment Variables` > `Path` > `New` e adicione o caminho `C:\php`;
	2. Abra o cmd do windows e digite `php --version`. Deve retornar a versão do php;
	3. Execute o notepad como administrador, clique em `File` > `Open` > `C:\Windows\System32\drivers\etc` > `todas as extensões` > `hosts.old`;
	4. Remova o comentário `#` da linha `127.0.0.1 localhost`. Se não tiver essa linha, basta adicioná-la;
6. Para rodar o servidor, acesse a pasta do projeto e digite no terminal: `php -S localhost:8000`;

Fonte: https://www.youtube.com/watch?v=HzIXZVctwI8
