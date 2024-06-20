<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LÓGICA DE PROGRAMAÇÃO - Atividade Avaliativa 1</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        h1, h2 {
            color: #333;
            text-align: center;
        }
        h3 {
            color: #333;
        }
        .question {
            margin-bottom: 20px;
        }
        .result {
            margin-top: 10px;
            font-weight: bold;
        }
        .footer {
            margin-top: 40px;
            font-size: 12px;
            text-align: center;
            color: #888;
        }
    </style>
    <script>
        function checkAnswer(questionId, correctAnswer) {
            var options = document.getElementsByName(questionId);
            var isCorrect = false;
            for (var i = 0; i < options.length; i++) {
                if (options[i].checked) {
                    if (options[i].value === correctAnswer) {
                        isCorrect = true;
                    }
                    break;
                }
            }
            var resultDiv = document.getElementById('result-' + questionId);
            if (isCorrect) {
                resultDiv.innerText = "Correto!";
                resultDiv.style.color = "green";
            } else {
                resultDiv.innerText = "Incorreto";
                resultDiv.style.color = "red";
            }
        }
    </script>
</head>
<body>
    <h1>LÓGICA DE PROGRAMAÇÃO</h1>
    <h2>Atividade Avaliativa 1</h2>

    <div class="question">
        <h3>QUESTÃO 1 DE 5: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
        <p>Sabendo que A = 3, B = 5 e C = 2. Cada uma das combinações abaixo será [V] Verdadeiro ou [F] Falso. Das alternativas abaixo, selecione aquela que representa a sequência correta de Verdadeiro e Falsos, lembrando que para chegar na resposta será necessário substituir as letras A, B e C pelos valores numéricos.</p>
        <p>(A + C) > B =<br>
        B >= (A + 2) =<br>
        C = (B – A) =<br>
        (B + A) <= C =<br>
        (C + A) > B =</p>
        <form id="question1">
            <label><input type="radio" name="question1" value="A"> A) [ F ] [ F ] [ V ] [ F ] [ F ]</label><br>
            <label><input type="radio" name="question1" value="B"> B) [ F ] [ V ] [ F ] [ V ] [ F ]</label><br>
            <label><input type="radio" name="question1" value="C"> C) [ F ] [ V ] [ V ] [ F ] [ F ]</label><br>
            <label><input type="radio" name="question1" value="D"> D) [ F ] [ V ] [ F ] [ V ] [ V ]</label><br>
            <label><input type="radio" name="question1" value="E"> E) [ V ] [ V ] [ V ] [ F ] [ F ]</label><br>
            <button type="button" onclick="checkAnswer('question1', 'C')">Verificar Resposta</button>
        </form>
        <div id="result-question1" class="result"></div>
    </div>

    <div class="question">
        <h3>QUESTÃO 2 DE 5: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
        <p>"Trata-se de uma forma de executar blocos de comandos somente sob determinadas condições, mas com a opção de repetir o mesmo bloco quantas vezes for necessário". Sobre qual estrutura diz este trecho:</p>
        <form id="question2">
            <label><input type="radio" name="question2" value="A"> A) Estrutura Operacional.</label><br>
            <label><input type="radio" name="question2" value="B"> B) Estrutura condicional.</label><br>
            <label><input type="radio" name="question2" value="C"> C) Estrutura de decisão.</label><br>
            <label><input type="radio" name="question2" value="D"> D) Estrutura de Repetição.</label><br>
            <label><input type="radio" name="question2" value="E"> E) Estrutura Validação.</label><br>
            <button type="button" onclick="checkAnswer('question2', 'D')">Verificar Resposta</button>
        </form>
        <div id="result-question2" class="result"></div>
    </div>

    <div class="question">
        <h3>QUESTÃO 3 DE 5: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
        <p>Assinale a Alternativa Correta sobre Variáveis.</p>
        <form id="question3">
            <label><input type="radio" name="question3" value="A"> A) Um espaço de memória do computador utilizado para guardar muitas informações simultaneamente.</label><br>
            <label><input type="radio" name="question3" value="B"> B) Uma palavra criada que pode armazenar várias informações ao mesmo tempo.</label><br>
            <label><input type="radio" name="question3" value="C"> C) Figuras utilizadas para definir um fluxograma.</label><br>
            <label><input type="radio" name="question3" value="D"> D) Um espaço de memória do computador para armazenar um tipo de dado determinado.</label><br>
            <label><input type="radio" name="question3" value="E"> E) Linguagem simbólica que apresenta como programa vai funcionar.</label><br>
            <button type="button" onclick="checkAnswer('question3', 'D')">Verificar Resposta</button>
        </form>
        <div id="result-question3" class="result"></div>
    </div>

    <div class="question">
        <h3>QUESTÃO 4 DE 5: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
        <p>As 3 fases fundamentais de um Algoritmo são:</p>
        <form id="question4">
            <label><input type="radio" name="question4" value="A"> A) ENTRADA-PROCESSAMENTO-SAÍDA.</label><br>
            <label><input type="radio" name="question4" value="B"> B) CÁLCULOS-PROCESSAMENTO-ENTRADA.</label><br>
            <label><input type="radio" name="question4" value="C"> C) VARIÁVEIS-CÁLCULOS-FLUXOGRAMAS.</label><br>
            <label><input type="radio" name="question4" value="D"> D) RECEBIMENTO-LOGICA-RESULTADO.</label><br>
            <label><input type="radio" name="question4" value="E"> E) LEITURA-TESTES-RESULTADOS.</label><br>
            <button type="button" onclick="checkAnswer('question4', 'A')">Verificar Resposta</button>
        </form>
        <div id="result-question4" class="result"></div>
    </div>

    <div class="question">
        <h3>QUESTÃO 5 DE 5: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
        <p>Assinale a Alternativa Correta sobre Lógica de Programação.</p>
        <form id="question5">
            <label><input type="radio" name="question5" value="A"> A) É uma sequência de passos que não segue nenhuma lógica.</label><br>
            <label><input type="radio" name="question5" value="B"> B) Emprego das operações matemáticas para chegar a um objetivo.</label><br>
            <label><input type="radio" name="question5" value="C"> C) Conjunto de regras para conseguir algo.</label><br>
            <label><input type="radio" name="question5" value="D"> D) É a técnica de Encadear pensamentos para chegar a um determinado objetivo.</label><br>
            <label><input type="radio" name="question5" value="E"> E) É a técnica de comparar informações com Verdadeiro ou Falso para chegar a uma conclusão.</label><br>
            <button type="button" onclick="checkAnswer('question5', 'D')">Verificar Resposta</button>
        </form>
        <div id="result-question5" class="result"></div>
    </div>

    <div class="footer">
        Simulador criado por Wellington Neri
    </div>
</body>
</html>
