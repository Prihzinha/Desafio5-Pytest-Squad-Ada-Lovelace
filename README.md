![Logo](https://blog.geekhunter.com.br/wp-content/uploads/2022/01/ada-lovelace-2.jpg)


# Turma 2 | Bootcamp Back-End Python e Django

## Squad Ada Lovelace

O grupo leva o nome de Augusta Ada Byron King, Condessa de Lovelace, atualmente conhecida como Ada Lovelace, foi uma matemática e escritora inglesa. Hoje é reconhecida principalmente por ter escrito o primeiro algoritmo para ser processado por uma máquina, a máquina analítica de Charles Babbage.


## Autoras

- [Amanda Savazzi](https://www.github.com/amandaspavan)
- [Brunna Victória](https://github.com/Brunnavic)
- [Caroline Teixeira](https://www.github.com/braincoreBR)
- [Juliana Thais](https://www.github.com/JulianaThais)
- [Jaqueline Santos](https://www.github.com/JaquelineAPSantos)
- [Kássia Oliveira](https://www.github.com/kmro)
- [Luana Gomes](https://www.github.com/luanafernanda)
- [Lorrane de Alkimim](https://www.github.com/LorraneAlkimim)
- [Melissa Oliveira](https://www.github.com/melissaoliveiras)
- [Priscila Rodrigues](https://www.github.com/Prihzinha)
- [Shomara Flores](https://www.github.com/ShomaraQuispe)


## Explicação do código

1-Introdução-a-testes-no-Python
Este código implementa uma função str_to_bool que converte uma string em um booleano. Ele considera algumas strings específicas como verdadeiras ('y', 'yes') e outras como falsas ('no', 'n'). Além disso, inclui testes unitários usando o módulo unittest para garantir o comportamento esperado da função. Os testes verificam se 'y' e 'Yes' são convertidos corretamente para verdadeiro e se a função levanta uma exceção AttributeError ao receber uma entrada inválida que não é uma string.


2-Fazer-testes-com-Pytest
Este código implementa uma função admin_command que adiciona o prefixo sudo a um comando, a menos que explicitamente não seja necessário. A função espera que command seja uma lista. O teste de unidade é realizado usando o módulo pytest para verificar se a função funciona corretamente em diferentes cenários:

test_no_sudo: Verifica se o comando não é prefixado com sudo quando sudo é definido como False.
test_sudo: Verifica se o comando é prefixado com sudo quando sudo é definido como True.
test_non_list_commands: Garante que a função levante um erro TypeError se o comando não for uma lista.


3-Teste-Avançado-com-Pytest
Este código contém testes e fixtures para várias funcionalidades, usando o framework pytest:

str_to_bool: Uma função que converte strings em valores booleanos, sendo testada com parâmetros usando @pytest.mark.parametrize:

test_str_to_bool_true: Verifica se strings representando "verdadeiro" (como 'Y', 'y', '1', 'YES') retornam True.
test_str_to_bool_false: Verifica se strings representando "falso" (como 'N', 'n', '0', 'NO') retornam False.
TestFile: Uma classe de teste que demonstra o uso de fixtures.

tmpfile: Uma fixture que cria um arquivo temporário e retorna seu caminho.
test_done_file: Verifica se um arquivo /tmp/done existe e contém o valor "1".
test_f: Usa a fixture tmpfile para criar um arquivo temporário, verifica se ele existe e contém o valor "1".

