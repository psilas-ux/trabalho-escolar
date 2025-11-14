<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Uso de condicionais para calcular capacidades</title>
    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #f4f4f4;
            margin: 0;
            padding: 20px;
        }
        .container {
            max-width: 900px;
            background: #fff;
            margin: auto;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        h1, h2, h3 {
            color: #005b9f;
        }
        pre {
            background: #eee;
            padding: 15px;
            border-radius: 5px;
            overflow-x: auto;
        }
        .code {
            background: #272822;
            color: #f8f8f2;
            padding: 15px;
            border-radius: 5px;
            font-family: Consolas, monospace;
        }
        ul {
            line-height: 1.7;
        }
    </style>
</head>
<body>

<div class="container">

    <h1>Uso de condicionais para calcular capacidades</h1>

    <h2>Introdução ao desafio</h2>
    <p>O desafio consiste em desenvolver um programa em Python que verifica se alunos e monitores podem ser transportados juntos em um bondinho com capacidade de até 50 pessoas.</p>

    <h2>Apresentação do desafio</h2>
    <p>O programa deve ler a quantidade de alunos e monitores e verificar se todos podem subir no bondinho em uma única viagem.</p>
    <p>Se o total de pessoas for menor ou igual a 50, todos podem ir juntos. Caso contrário, será necessário fazer mais de uma viagem.</p>

    <h2>Valores de entrada</h2>
    <ul>
        <li>Quantidade de alunos</li>
        <li>Quantidade de monitores</li>
    </ul>

    <h2>Início da programação</h2>
    <p>Os valores devem ser informados pelo usuário usando <strong>input()</strong>, convertidos para números inteiros usando <strong>int()</strong>.</p>

    <h3>Código para entrada de dados:</h3>
    <pre class="code">numero_de_alunos = int(input("Digite a quantidade de alunos: "))
numero_de_monitores = int(input("Digite a quantidade de monitores: "))</pre>

    <h2>Estrutura condicional</h2>
    <p>O programa precisa verificar se o total de pessoas cabe no bondinho de 50 lugares.</p>

    <h3>Condição usada:</h3>
    <pre class="code">if numero_de_alunos + numero_de_monitores <= 50:</pre>

    <h2>Definição das respostas</h2>
    <pre class="code">resposta_positiva = "pode ir"
resposta_negativa = "não pode ir"</pre>

    <h2>Implementação completa</h2>
    <pre class="code">if numero_de_alunos + numero_de_monitores <= 50:
    print(resposta_positiva)
else:
    print(resposta_negativa)</pre>

    <h2>Teste do código</h2>
    <p><strong>Exemplo 1:</strong> 55 alunos e 10 monitores → total = 65 → “não pode ir”.</p>
    <p><strong>Exemplo 2:</strong> 10 alunos e 10 monitores → total = 20 → “pode ir”.</p>

    <h2>Desafio adicional</h2>
    <p>Agora existe um novo bondinho com capacidade de 30 pessoas e também haverá 8 professores.</p>

    <p>O programa deve verificar se alunos, monitores e 8 professores cabem no bondinho.</p>

    <h3>Enunciado do novo desafio:</h3>
    <pre class="code">capacidade = 30
professores = 8

alunos = int(input("Digite o número de alunos: "))
monitores = int(input("Digite o número de monitores: "))

total = alunos + monitores + professores

if total <= capacidade:
    print("pode ir")
else:
    print("não pode ir")</pre>

</div>

</body>
</html>
