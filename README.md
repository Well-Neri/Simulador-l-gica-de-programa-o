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
        <h3>QUESTÃO 1 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
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
        <h3>QUESTÃO 2 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
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
        <h3>QUESTÃO 3 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
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
        <h3>QUESTÃO 4 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
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
        <h3>QUESTÃO 5 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
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

  <div class="question">
    <h3>QUESTÃO 6 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>A linguagem simbólica que apresentamos como o programa vai funcionar denominamos:</p>
    <form id="question6">
        <label><input type="radio" name="question6" value="A"> A) Fluxograma.</label><br>
        <label><input type="radio" name="question6" value="B"> B) Programa objeto.</label><br>
        <label><input type="radio" name="question6" value="C"> C) Programa fonte.</label><br>
        <label><input type="radio" name="question6" value="D"> D) Algoritmo.</label><br>
        <label><input type="radio" name="question6" value="E"> E) Código aberto.</label><br>
        <button type="button" onclick="checkAnswer('question6', 'A')">Verificar Resposta</button>
    </form>
    <div id="result-question6" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 7 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>Qual Estrutura de Decisão se enquadra com o Fluxograma abaixo:</p>
    <img src="https://img.uninove.br/static/0/0/0/0/0/0/4/9/2/8/4/4928438/q2-at2.jpg" alt="Fluxograma" style="width:100%; max-width:400px;">
    <form id="question7">
        <label><input type="radio" name="question7" value="A"> A) Estrutura de Decisão Simples.</label><br>
        <label><input type="radio" name="question7" value="B"> B) Estrutura de Decisão Encadeada.</label><br>
        <label><input type="radio" name="question7" value="C"> C) Estrutura de Decisão Sequencial.</label><br>
        <label><input type="radio" name="question7" value="D"> D) Estrutura de Decisão Espiral.</label><br>
        <label><input type="radio" name="question7" value="E"> E) Estrutura de Decisão Composta.</label><br>
        <button type="button" onclick="checkAnswer('question7', 'A')">Verificar Resposta</button>
    </form>
    <div id="result-question7" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 8 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>Qual Estrutura de Decisão se enquadra com o Fluxograma abaixo:</p>
    <img src="https://img.uninove.br/static/0/0/0/0/0/0/4/9/2/8/4/4928437/q3-at2.jpg" alt="Fluxograma" style="width:100%; max-width:400px;">
    <form id="question8">
        <label><input type="radio" name="question8" value="A"> A) Estrutura de Decisão Simples.</label><br>
        <label><input type="radio" name="question8" value="B"> B) Estrutura de Decisão Espiral.</label><br>
        <label><input type="radio" name="question8" value="C"> C) Estrutura de Decisão Encadeada.</label><br>
        <label><input type="radio" name="question8" value="D"> D) Estrutura de Decisão Sequencial.</label><br>
        <label><input type="radio" name="question8" value="E"> E) Estrutura de Decisão Composta.</label><br>
        <button type="button" onclick="checkAnswer('question8', 'E')">Verificar Resposta</button>
    </form>
    <div id="result-question8" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 9 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>Considerando A = 10, B = 7 e C = 6, assinale a opção correta relacionada à lógica de programação.</p>
    <form id="question9">
        <label><input type="radio" name="question9" value="A"> A) (A + 3) > (B + C)</label><br>
        <label><input type="radio" name="question9" value="B"> B) ((B * 4) >= (A + A * 2) AND (5 + 5) >= (A))</label><br>
        <label><input type="radio" name="question9" value="C"> C) ((A + C) < (B * 2) OR (C + B * 3) < (A * 3))</label><br>
        <label><input type="radio" name="question9" value="D"> D) (C * 3) <= (3 + C * 2)</label><br>
        <label><input type="radio" name="question9" value="E"> E) ((B + A) > (C + C) AND (A - C) < (B - A))</label><br>
        <button type="button" onclick="checkAnswer('question9', 'C')">Verificar Resposta</button>
    </form>
    <div id="result-question9" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 10 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>Um algoritmo é:</p>
    <form id="question10">
        <label><input type="radio" name="question10" value="A"> A) A parte de um programa em que se limita a definir as constantes.</label><br>
        <label><input type="radio" name="question10" value="B"> B) A operação matemática inversa a potência.</label><br>
        <label><input type="radio" name="question10" value="C"> C) Um software utilizado para escrever programas.</label><br>
        <label><input type="radio" name="question10" value="D"> D) Uma sequência de passos para realizar uma atividade.</label><br>
        <label><input type="radio" name="question10" value="E"> E) A parte de um programa em que se limita a definir os tipos de dados das variáveis.</label><br>
        <button type="button" onclick="checkAnswer('question10', 'D')">Verificar Resposta</button>
    </form>
    <div id="result-question10" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 11 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>No contexto do comando switch e do uso do comando break em seu interior, na linguagem de programação C, é correto afirmar que:</p>
    <form id="question11">
        <label><input type="radio" name="question11" value="A"> A) A expressão usada numa cláusula case de um comando switch pode ser de qualquer tipo e deve conter pelo menos uma variável;</label><br>
        <label><input type="radio" name="question11" value="B"> B) Não é possível executar comandos de uma das cláusulas case de um comando switch na mesma execução desse comando;</label><br>
        <label><input type="radio" name="question11" value="C"> C) Quando um comando break é executado, o comando switch é encerrado e o fluxo de controle passa para o próximo comando após o fim do comando switch;</label><br>
        <label><input type="radio" name="question11" value="D"> D) Toda cláusula case de um comando switch, incluindo a cláusula case default, deve conter um comando break;</label><br>
        <label><input type="radio" name="question11" value="E"> E) Os comandos na cláusula case default de um comando switch são executados apenas se nenhuma das cláusulas case anteriores possuir um comando break;</label><br>
        <button type="button" onclick="checkAnswer('question11', 'C')">Verificar Resposta</button>
    </form>
    <div id="result-question11" class="result"></div>
</div>


<div class="question">
    <h3>QUESTÃO 12 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>Considere o seguinte programa em anexo, escrito em C:</p>
    <img src="https://img.uninove.br/static/0/0/0/0/0/0/7/2/2/0/1/7220169/2.jpg" alt="Fluxograma" style="width:100%; max-width:400px;">
    <p>Após a execução do programa, o que aparecerá na tela será?:</p>    
    <form id="question12">
        <label><input type="radio" name="question12" value="A"> A) x=0, y=25, z=5</label><br>
        <label><input type="radio" name="question12" value="B"> B) x=0, y=5, z=5</label><br>
        <label><input type="radio" name="question12" value="C"> C) x=25, y=0, z=25</label><br>
        <label><input type="radio" name="question12" value="D"> D) x=5, y=0, z=25</label><br>
        <label><input type="radio" name="question12" value="E"> E) x=5, y=5, z=5</label><br>
        <button type="button" onclick="checkAnswer('question12', 'B')">Verificar Resposta</button>
    </form>
    <div id="result-question12" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 13 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>Operadores lógicos servem para combinar resultados de expressões, cujo resultado será verdadeiro ou falso. Assinale a alternativa CORRETA conforme as expressões abaixo:</p>
        <form id="question13">
        <label><input type="radio" name="question13" value="A"> A) Verdadeiro AND Falso = Verdadeiro.</label><br>
        <label><input type="radio" name="question13" value="B"> B) Verdadeiro OR Verdadeiro = Falso.</label><br>
        <label><input type="radio" name="question13" value="C"> C) Falso OR Verdadeiro = Verdadeiro.</label><br>
        <label><input type="radio" name="question13" value="D"> D) Verdadeiro AND Verdadeiro = Falso.</label><br>
        <label><input type="radio" name="question13" value="E"> E) Verdadeiro NOT = Verdadeiro.</label><br>
        <button type="button" onclick="checkAnswer('question13', 'C')">Verificar Resposta</button>
    </form>
    <div id="result-question13" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 14 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>Que opção usamos no comando switch na linguagem C para executar um comando, se nenhum comando das opções case for executada? </p>
        <form id="question14">
        <label><input type="radio" name="question14" value="A"> A) switch.</label><br>
        <label><input type="radio" name="question14" value="B"> B) else.</label><br>
        <label><input type="radio" name="question14" value="C"> C) case.</label><br>
        <label><input type="radio" name="question14" value="D"> D) default.</label><br>
        <label><input type="radio" name="question14" value="E"> E) break.</label><br>
        <button type="button" onclick="checkAnswer('question14', 'D')">Verificar Resposta</button>
    </form>
    <div id="result-question14" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 15 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>Em programação C, o comando while:</p>
        <form id="question15">
        <label><input type="radio" name="question15" value="A"> A) Equivale ao comando what-if.</label><br>
        <label><input type="radio" name="question15" value="B"> B) Executa um bloco de comandos enquanto sua condição for verdadeira.</label><br>
        <label><input type="radio" name="question15" value="C"> C) É idêntico ao comando do while.</label><br>
        <label><input type="radio" name="question15" value="D"> D) Executa um bloco exclusivamente de comandos de atribuição.</label><br>
        <label><input type="radio" name="question15" value="E"> E) Executa um bloco de comandos até que sua condição seja verdadeira.</label><br>
        <button type="button" onclick="checkAnswer('question15', 'B')">Verificar Resposta</button>
    </form>
    <div id="result-question15" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 16 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>Sabe-se que as variáveis Parte1 e Parte2 são do tipo de dado string. Para cada uma, foram atribuídos “Neide” e “Linda” respectivamente. Uma terceira variável Mensagem do tipo de dado string foi utilizada e o seu conteúdo após o processamento do programa é “LindaNeide”. Sabe-se também que o conteúdo da variável Mensagem foi obtido a partir das variáveis Parte1 e Parte2. Marque a alternativa que representa a codificação da variável Mensagem que tem como conteúdo “LindaNeide”.</p>
        <form id="question16">
        <label><input type="radio" name="question16" value="A"> A) Mensagem = Parte2 + Parte1;</label><br>
        <label><input type="radio" name="question16" value="B"> B) Mensagem = “Parte1” + “  ” + “Parte2”;</label><br>
        <label><input type="radio" name="question16" value="C"> C) Mensagem = Parte2 “  ” Parte1;</label><br>
        <label><input type="radio" name="question16" value="D"> D) Mensagem = Parte1 + Parte2;</label><br>
        <label><input type="radio" name="question16" value="E"> E) Mensagem = “Parte1” + “Parte2”;</label><br>
        <button type="button" onclick="checkAnswer('question16', 'A')">Verificar Resposta</button>
    </form>
    <div id="result-question16" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 17 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>O valor da variável R é obtido a partir do processamento de: R = ( ( n2 + n1 ) / 2 ) * n3; Marque a alternativa que indica o valor da variável R.</p>
        <form id="question17">
        <label><input type="radio" name="question17" value="A"> A) 270.</label><br>
        <label><input type="radio" name="question17" value="B"> B) 126.</label><br>
        <label><input type="radio" name="question17" value="C"> C) 180.</label><br>
        <label><input type="radio" name="question17" value="D"> D) 450.</label><br>
        <label><input type="radio" name="question17" value="E"> E) 360.</label><br>
        <button type="button" onclick="checkAnswer('question17', 'A')">Verificar Resposta</button>
    </form>
    <div id="result-question17" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 18 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>Analise o trecho do código em anexo:</p>
    <img src="https://img.uninove.br/static/0/0/0/0/0/0/7/2/2/0/5/7220514/3.jpg" style="width:100%; max-width:400px;">
    <p>Após a execução do código, qual será o valor da variável c?</p>
        <form id="question18">
        <label><input type="radio" name="question18" value="A"> A) 5.</label><br>
        <label><input type="radio" name="question18" value="B"> B) 2.</label><br>
        <label><input type="radio" name="question18" value="C"> C) 12.</label><br>
        <label><input type="radio" name="question18" value="D"> D) 10.</label><br>
        <label><input type="radio" name="question18" value="E"> E) 15.</label><br>
        <button type="button" onclick="checkAnswer('question18', 'D')">Verificar Resposta</button>
    </form>
    <div id="result-question18" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 19 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>Considere as seguintes linhas de código para responder as questões a seguir: int varValor1 = 2; int varValor2 = 10; Marque a alternativa que representa o valor 20 obtido a partir das variáveis apresentadas.</p>
        <form id="question19">
        <label><input type="radio" name="question19" value="A"> A) var(Valor1 * Valor2)</label><br>
        <label><input type="radio" name="question19" value="B"> B) varValor2 * 2 * varValor1 * 10</label><br>
        <label><input type="radio" name="question19" value="C"> C) 2 * 20</label><br>
        <label><input type="radio" name="question19" value="D"> D) varValor1 * varValor2</label><br>
        <label><input type="radio" name="question19" value="E"> E) Valor1 * Valor2</label><br>
        <button type="button" onclick="checkAnswer('question19', 'D')">Verificar Resposta</button>
    </form>
    <div id="result-question19" class="result"></div>
</div>

<div class="question">
    <h3>QUESTÃO 20 DE 20: ATIVIDADE DE MÚLTIPLA ESCOLHA</h3>
    <p>Conforme o código em anexo, em qual categoria o Nadador se encaixa.</p>
    <img src="https://img.uninove.br/static/0/0/0/0/0/0/7/2/2/0/5/7220515/5.jpg" style="width:100%; max-width:400px;">
    <form id="question20">
        <label><input type="radio" name="question20" value="A"> A) Juvenil A.</label><br>
        <label><input type="radio" name="question20" value="B"> B) Juvenil B.</label><br>
        <label><input type="radio" name="question20" value="C"> C) Infantil A.</label><br>
        <label><input type="radio" name="question20" value="D"> D) Infantil B.</label><br>
        <label><input type="radio" name="question20" value="E"> E) Ops você ainda não pode ser um nadador!</label><br>
        <button type="button" onclick="checkAnswer('question20', 'E')">Verificar Resposta</button>
    </form>
    <div id="result-question20" class="result"></div>
</div>


    <div class="footer">
        Simulador criado por Wellington Neri
    </div>
</body>
</html>
