# 1. Instruções condicionais básicas

## Exercício 1 --- Número Positivo, Negativo ou Nulo

**Enunciado:** Ler um número inteiro e indicar se é positivo, negativo
ou nulo.

    Dados de entrada Resultado esperado
  ------------------ --------------------
                 `8` Positivo
                `-3` Negativo
                 `0` Nulo

## Exercício 2 --- Classificação por Idade

**Enunciado:** Ler uma idade (inteiro) e classificá-la como criança
(menos de 12 anos), adolescente (12--17 anos), adulto (18--64 anos) ou
sénior (65 anos ou mais).

    Dados de entrada (idade) Resultado esperado
  -------------------------- --------------------
                         `7` Criança
                        `12` Adolescente
                        `17` Adolescente
                        `18` Adulto
                        `64` Adulto
                        `65` Sénior

## Exercício 3 --- Classificação da Temperatura

**Enunciado:** Ler uma temperatura em graus Celsius (real) e
classificá-la como gelada (≤ 0), fria (\> 0 e \< 15), amena (15--25) ou
quente (\> 25).

    Dados de entrada (°C) Resultado esperado
  ----------------------- --------------------
                     `-4` Gelada
                      `0` Gelada
                    `0.5` Fria
                   `14.9` Fria
                     `15` Amena
                     `25` Amena
                   `25.1` Quente

## Exercício 4 --- Classificação de uma Nota

**Enunciado:** Ler uma nota entre 0 e 20 (real). Classificá-la como
insuficiente (\< 10), suficiente (10--13), bom (14--16), muito bom
(17--18) ou excelente (19--20). Rejeitar valores fora do intervalo
válido.

    Dados de entrada (nota) Resultado esperado
  ------------------------- --------------------
                       `-1` Nota inválida
                        `0` Insuficiente
                      `9.9` Insuficiente
                       `10` Suficiente
                     `13.5` Suficiente
                       `14` Bom
                     `16.5` Bom
                       `17` Muito bom
                     `18.9` Muito bom
                       `19` Excelente
                       `20` Excelente
                     `20.1` Nota inválida

## Exercício 5 --- Maior de Três Números

**Enunciado:** Ler três números inteiros e apresentar o maior. Se dois
ou três valores forem iguais ao maior, apresentar esse valor.

  Dados de entrada (a, b, c)     Resultado esperado
  ---------------------------- --------------------
  `4, 9, 2`                              Maior: `9`
  `10, 3, 7`                            Maior: `10`
  `1, 2, 8`                              Maior: `8`
  `5, 5, 2`                              Maior: `5`
  `6, 6, 6`                              Maior: `6`
  `-4, -2, -9`                          Maior: `-2`

## Exercício 6 --- Sistema de Autenticação Simples

**Enunciado:** Ler um nome de utilizador e uma palavra-passe (cadeias de
caracteres). O nome de utilizador correto é `admin` e a palavra-passe
correta é `1234`.

  -----------------------------------------------------------------------
  Dados de entrada (utilizador,       Resultado esperado
  palavra-passe)                      
  ----------------------------------- -----------------------------------
  `admin`, `1234`                     Autenticação bem-sucedida

  `admin`, `wrong`                    Autenticação sem sucesso

  `guest`, `1234`                     Autenticação sem sucesso

  `guest`, `wrong`                    Autenticação sem sucesso

  `Admin`, `1234`                     Autenticação sem sucesso
                                      (comparação sensível a
                                      maiúsculas/minúsculas)
  -----------------------------------------------------------------------

## Exercício 7 --- Custo de Envio

**Enunciado:** Ler o peso de uma encomenda em quilogramas (real). Custo:
até 1 kg = 3,50 €; mais de 1 e até 5 kg = 6,00 €; mais de 5 e até 10 kg
= 10,00 €; mais de 10 kg = 15,00 €. Rejeitar pesos nulos ou negativos.

    Dados de entrada (kg) Resultado esperado
  ----------------------- -------------------------
                      `0` Peso inválido
                    `0.5` Custo de envio: 3,50 €
                      `1` Custo de envio: 3,50 €
                   `1.01` Custo de envio: 6,00 €
                      `5` Custo de envio: 6,00 €
                    `5.1` Custo de envio: 10,00 €
                     `10` Custo de envio: 10,00 €
                   `10.1` Custo de envio: 15,00 €

## Exercício 8 --- Consumo de Eletricidade

**Enunciado:** Ler o consumo mensal em kWh (real). Classificá-lo como
baixo (\< 100), moderado (100--300), elevado (\> 300--500) ou muito
elevado (\> 500).

    Dados de entrada (kWh) Resultado esperado
  ------------------------ --------------------
                      `75` Baixo
                     `100` Moderado
                     `250` Moderado
                     `300` Moderado
                   `300.1` Elevado
                     `500` Elevado
                   `500.1` Muito elevado

------------------------------------------------------------------------

# 2. Instruções condicionais com várias variáveis

## Exercício 9 --- Classificação de Triângulos

**Enunciado:** Ler os comprimentos de três lados (reais). Um triângulo é
válido apenas se todos os lados forem positivos e a soma de quaisquer
dois lados for superior ao terceiro. Se for válido, classificá-lo como
equilátero, isósceles ou escaleno.

  Dados de entrada (a, b, c)   Resultado esperado
  ---------------------------- -----------------------
  `3, 3, 3`                    Válido --- Equilátero
  `5, 5, 8`                    Válido --- Isósceles
  `3, 4, 5`                    Válido --- Escaleno
  `1, 2, 3`                    Triângulo inválido
  `1, 2, 4`                    Triângulo inválido
  `0, 4, 4`                    Triângulo inválido
  `-2, 4, 4`                   Triângulo inválido

## Exercício 10 --- Preço de Bilhetes de Cinema

**Enunciado:** Ler a idade (inteiro) e a indicação de estudante (`yes`
ou `no`). Preços-base: menos de 12 anos = 5,00 €; dos 12 aos 64 anos =
10,00 €; 65 anos ou mais = 6,00 €. Os estudantes têm um desconto de 20%
sobre o preço aplicável.

  Dados de entrada (idade, estudante?)     Resultado esperado
  -------------------------------------- --------------------
  `10, no`                                             5,00 €
  `10, yes`                                            4,00 €
  `25, no`                                            10,00 €
  `25, yes`                                            8,00 €
  `64, yes`                                            8,00 €
  `65, no`                                             6,00 €
  `70, yes`                                            4,80 €

## Exercício 11 --- Ponto no Interior de um Retângulo

**Enunciado:** Ler os limites do retângulo (`xmin`, `xmax`, `ymin`,
`ymax`) e as coordenadas de um ponto (`x`, `y`), todos reais. Assumir
que os limites do retângulo são introduzidos pela ordem correta.
Determinar se o ponto está no interior, no exterior ou sobre a fronteira
do retângulo.

  Dados de entrada (xmin, xmax, ymin, ymax; x, y)   Resultado esperado
  ------------------------------------------------- --------------------
  `0, 10, 0, 5; 5, 2`                               Interior
  `0, 10, 0, 5; -1, 2`                              Exterior
  `0, 10, 0, 5; 10, 2`                              Sobre a fronteira
  `0, 10, 0, 5; 5, 0`                               Sobre a fronteira
  `0, 10, 0, 5; 10, 5`                              Sobre a fronteira
  `0, 10, 0, 5; 11, 6`                              Exterior

## Exercício 12 --- Bónus Salarial de um Funcionário

**Enunciado:** Ler o salário mensal (real), os anos de serviço (inteiro)
e a avaliação de desempenho (`excellent`, `good` ou `average`). Bónus:
desempenho excelente e ≥ 5 anos = 20%; excelente e \< 5 anos = 15%; bom
e ≥ 5 anos = 10%; bom e \< 5 anos = 5%; médio = 0%. Apresentar o valor
do bónus.

  Dados de entrada (salário, anos, desempenho)     Bónus esperado
  ---------------------------------------------- ----------------
  `2000, 5, excellent`                                   400,00 €
  `2000, 2, excellent`                                   300,00 €
  `2000, 5, good`                                        200,00 €
  `2000, 2, good`                                        100,00 €
  `2000, 10, average`                                      0,00 €
  `1500, 4, good`                                         75,00 €

------------------------------------------------------------------------

# 3. Ciclos while básicos

## Exercício 13 --- Contar de 1 até N

**Enunciado:** Ler um número inteiro positivo N e utilizar um ciclo
`while` para apresentar todos os números inteiros de 1 até N.

    Dados de entrada (N) Resultado esperado
  ---------------------- --------------------
                     `1` `1`
                     `5` `1 2 3 4 5`
                     `8` `1 2 3 4 5 6 7 8`

## Exercício 14 --- Contagem Decrescente

**Enunciado:** Ler um número inteiro inicial e apresentar a contagem
decrescente desse número até zero.

    Dados de entrada Resultado esperado
  ------------------ --------------------
                 `0` `0`
                 `1` `1 0`
                 `5` `5 4 3 2 1 0`
                 `3` `3 2 1 0`

## Exercício 15 --- Validação da Palavra-passe

**Enunciado:** Pedir repetidamente uma palavra-passe até que o
utilizador introduza `1234`.

  -----------------------------------------------------------------------
  Tentativas de palavra-passe (por    Resultado esperado
  ordem)                              
  ----------------------------------- -----------------------------------
  `1234`                              Mensagem de boas-vindas após 1
                                      tentativa

  `0000`, `1234`                      Palavra-passe incorreta; depois,
                                      mensagem de boas-vindas após 2
                                      tentativas

  `admin`, `pass`, `1234`             Duas mensagens de palavra-passe
                                      incorreta; depois, mensagem de
                                      boas-vindas após 3 tentativas
  -----------------------------------------------------------------------

## Exercício 16 --- Introdução de um Número Positivo

**Enunciado:** Pedir repetidamente um número real até que o utilizador
introduza um valor superior a zero.

  Tentativas de introdução (por ordem)   Resultado esperado
  -------------------------------------- -------------------------------------------------
  `2.5`                                  Aceite: `2.5`
  `0`, `4.2`                             Rejeitar `0`; aceitar `4.2`
  `-3`, `-0.5`, `7`                      Rejeitar os dois valores negativos; aceitar `7`

## Exercício 17 --- Classificação de Números

**Enunciado:** Ler exatamente 10 números inteiros. Para cada número,
indicar se é positivo, negativo ou nulo.

  -------------------------------------------------------------------------------
  Sequência de dados de entrada               Classificações esperadas (pela
                                              mesma ordem)
  ------------------------------------------- -----------------------------------
  `1, -1, 0, 2, -2, 3, -3, 4, -4, 5`          Positivo, Negativo, Nulo, Positivo,
                                              Negativo, Positivo, Negativo,
                                              Positivo, Negativo, Positivo

  `0, 0, 0, 0, 0, 0, 0, 0, 0, 0`              Nulo para os 10 valores

  `-1, -2, -3, -4, -5, -6, -7, -8, -9, -10`   Negativo para os 10 valores
  -------------------------------------------------------------------------------

## Exercício 18 --- Monitorização da Temperatura

**Enunciado:** Ler temperaturas repetidamente. Apresentar Fria (\< 15
°C), Confortável (15--25 °C) ou Quente (\> 25 °C). Terminar quando o
utilizador introduzir `-999`; não classificar esse valor de controlo.

  Sequência de temperaturas   Resultado esperado
  --------------------------- -------------------------------------------
  `10, 20, 30, -999`          Fria; Confortável; Quente; terminar
  `15, 25, -999`              Confortável; Confortável; terminar
  `-999`                      Terminar imediatamente; sem classificação
  `0, 14.9, 25.1, -999`       Fria; Fria; Quente; terminar

------------------------------------------------------------------------

# 4. Combinação de ciclos while e instruções condicionais

## Exercício 19 --- Simulação de Levantamento numa Caixa Multibanco

**Enunciado:** Começar com um saldo de 1000 €. Pedir repetidamente um
montante a levantar. O valor `0` termina o programa. Rejeitar montantes
negativos; apresentar uma mensagem de saldo insuficiente se o montante
for superior ao saldo; caso contrário, subtrair o montante e apresentar
o novo saldo.

  -----------------------------------------------------------------------
  Sequência de levantamentos          Resultado esperado
  ----------------------------------- -----------------------------------
  `100, 200, 0`                       Saldo: 900,00 €; depois 700,00 €;
                                      terminar

  `1000, 0`                           Saldo: 0,00 €; terminar

  `1200, 0`                           Saldo insuficiente; o saldo
                                      mantém-se em 1000,00 €; terminar

  `-50, 50, 0`                        Montante inválido; depois saldo:
                                      950,00 €; terminar

  `0`                                 Terminar imediatamente; saldo
                                      mantém-se em 1000,00 €
  -----------------------------------------------------------------------

## Exercício 20 --- Estatísticas das Notas de um Exame

**Enunciado:** Ler o número de alunos e, em seguida, a nota de cada
aluno (0--20). Contar as notas inferiores a 10 como reprovações e as
notas iguais ou superiores a 10 como aprovações. Apresentar ambas as
contagens.

  Número de alunos e respetivas notas   Resultado esperado
  ------------------------------------- -----------------------------
  `4; 8, 10, 15, 9`                     Aprovados: 2; Reprovados: 2
  `3; 10, 12, 20`                       Aprovados: 3; Reprovados: 0
  `3; 0, 4, 9.9`                        Aprovados: 0; Reprovados: 3
  `1; 9.99`                             Aprovados: 0; Reprovados: 1

## Exercício 21 --- Sistema de Pedidos de um Restaurante

**Enunciado:** Apresentar repetidamente um menu: hambúrguer 8,50 €,
pizza 10,00 €, salada 6,00 € e refrigerante 2,00 €. Adicionar as opções
válidas ao total. A opção `0` termina o pedido; as opções inválidas não
podem alterar o total.

  Sequência de opções   Resultado esperado
  --------------------- -----------------------------------
  `1, 2, 0`             Total: 18,50 €
  `3, 3, 4, 0`          Total: 14,00 €
  `0`                   Total: 0,00 €
  `5, 1, 0`             Opção `5` inválida; total: 8,50 €
  `1, 1, 1, 0`          Total: 25,50 €

## Exercício 22 --- Adivinhar o Número

**Enunciado:** Definir o número secreto como 42. Continuar a pedir
palpites até que seja introduzido o número correto. Apresentar
`Demasiado baixo!`, `Demasiado alto!` ou `Parabéns!`, conforme o caso.

  Sequência de palpites   Resultado esperado
  ----------------------- ----------------------------------------------
  `42`                    Parabéns!
  `20, 42`                Demasiado baixo!; Parabéns!
  `60, 42`                Demasiado alto!; Parabéns!
  `20, 50, 42`            Demasiado baixo!; Demasiado alto!; Parabéns!

## Exercício 23 --- Gestão de uma Conta Bancária

**Enunciado:** Começar com um saldo de 500 €. Menu: 1 Depositar, 2
Levantar, 3 Consultar saldo, 0 Sair. Os depósitos e levantamentos têm de
ser positivos; não é possível levantar um montante superior ao saldo.

  -----------------------------------------------------------------------
  Ações no menu (por ordem)           Resultado esperado
  ----------------------------------- -----------------------------------
  `3, 0`                              Apresentar saldo de 500,00 €; sair

  `1:100, 3, 0`                       Depósito aceite; apresentar saldo
                                      de 600,00 €; sair

  `2:200, 3, 0`                       Levantamento aceite; apresentar
                                      saldo de 300,00 €; sair

  `2:600, 3, 0`                       Saldo insuficiente; saldo mantém-se
                                      em 500,00 €; sair

  `1:-20, 3, 0`                       Depósito inválido; saldo mantém-se
                                      em 500,00 €; sair

  `2:0, 3, 0`                         Levantamento inválido; saldo
                                      mantém-se em 500,00 €; sair

  `9, 0`                              Opção de menu inválida; sair
  -----------------------------------------------------------------------

## Exercício 24 --- Análise do Preço de Produtos

**Enunciado:** Ler preços de produtos até ser introduzido o valor `-1`.
Rejeitar os restantes preços negativos. Classificar os preços válidos:
abaixo de 10 € --- barato; de 10 € a 50 €, inclusive --- preço moderado;
acima de 50 € --- caro. Apresentar o número de produtos válidos
introduzidos.

  -----------------------------------------------------------------------
  Sequência de preços                 Resultado esperado
  ----------------------------------- -----------------------------------
  `5, 10, 50, 60, -1`                 Baratos: 1; Moderados: 2; Caros: 1;
                                      Produtos: 4

  `-1`                                Produtos: 0

  `-5, 8, -1`                         Rejeitar `-5`; Baratos: 1;
                                      Produtos: 1

  `9.99, 10, 50.01, -1`               Baratos: 1; Moderados: 1; Caros: 1;
                                      Produtos: 3
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# 5. Exercícios de desafio

## Exercício 25 --- Sistema de Aluguer de Automóveis

**Enunciado:** Ler o nome do cliente (cadeia de caracteres), a categoria
do veículo (`economy`, `standard` ou `premium`), o número de dias de
aluguer (inteiro) e a idade (inteiro). Os preços diários são 25 €, 40 €
e 65 €, respetivamente. O cliente tem de ter pelo menos 21 anos e o
aluguer tem de durar pelo menos um dia. Os alugueres superiores a 7 dias
têm um desconto de 10%. Rejeitar categorias inválidas.

  -----------------------------------------------------------------------
  Dados de entrada (nome, categoria,  Resultado esperado
  dias, idade)                        
  ----------------------------------- -----------------------------------
  `Alex, economy, 3, 25`              Custo do aluguer: 75,00 €

  `Alex, standard, 7, 30`             Custo do aluguer: 280,00 €

  `Alex, premium, 8, 40`              Subtotal: 520,00 €; desconto: 52,00
                                      €; custo final: 468,00 €

  `Alex, economy, 10, 20`             Rejeitado: o cliente tem de ter
                                      pelo menos 21 anos

  `Alex, economy, 0, 25`              Rejeitado: a duração do aluguer tem
                                      de ser, pelo menos, 1 dia

  `Alex, luxury, 3, 25`               Rejeitado: categoria de veículo
                                      inválida

  `Alex, standard, 10, 21`            Subtotal: 400,00 €; desconto: 40,00
                                      €; custo final: 360,00 €
  -----------------------------------------------------------------------

## Exercício 26 --- Admissão à Universidade

**Enunciado:** Ler as notas de Matemática, Programação e Inglês (reais).
Os requisitos de admissão são: Matemática ≥ 12, Programação ≥ 14, Inglês
≥ 10 e média ≥ 13.

  -----------------------------------------------------------------------
  Dados de entrada (Matemática,       Resultado esperado
  Programação, Inglês)                
  ----------------------------------- -----------------------------------
  `12, 14, 13`                        Admitido (média: 13,00)

  `15, 16, 14`                        Admitido (média: 15,00)

  `11, 18, 15`                        Não admitido: requisito de
                                      Matemática não cumprido

  `18, 13, 15`                        Não admitido: requisito de
                                      Programação não cumprido

  `15, 18, 9`                         Não admitido: requisito de Inglês
                                      não cumprido

  `12, 14, 10`                        Não admitido: média de 12,00

  `20, 20, 20`                        Admitido (média: 20,00)
  -----------------------------------------------------------------------

## Exercício 27 --- Monitorização do Consumo de Combustível

**Enunciado:** Ler repetidamente a distância percorrida (km) e o
combustível consumido (litros). Uma distância de `-1` termina o
programa. Para dados válidos, calcular o consumo através da fórmula
`(combustível / distância) × 100`. Classificar valores inferiores a 5
como Económico, de 5 a 8, inclusive, como Normal e superiores a 8 como
Elevado. Rejeitar distâncias inválidas ou quantidades de combustível
inválidas.

  -----------------------------------------------------------------------
  Sequência de dados de entrada       Resultado esperado
  (distância, combustível)            
  ----------------------------------- -----------------------------------
  `(100, 4), (-1, —)`                 4,00 L/100 km --- Económico;
                                      terminar

  `(100, 6), (-1, —)`                 6,00 L/100 km --- Normal; terminar

  `(50, 5), (-1, —)`                  10,00 L/100 km --- Elevado;
                                      terminar

  `(0, 5), (100, 5), (-1, —)`         Rejeitar distância nula; depois
                                      5,00 L/100 km --- Normal; terminar

  `(100, -2), (100, 8), (-1, —)`      Rejeitar combustível negativo;
                                      depois 8,00 L/100 km --- Normal;
                                      terminar

  `(-1, —)`                           Terminar imediatamente; não efetuar
                                      cálculos
  -----------------------------------------------------------------------

## Exercício 28 --- Registo de Assiduidade dos Funcionários

**Enunciado:** Ler repetidamente o nome do funcionário, as horas
trabalhadas (real) e o número de faltas (inteiro). Terminar quando o
nome introduzido for `END`. Assiduidade: 0 faltas = assiduidade
perfeita; 1--2 faltas = boa assiduidade; mais de 2 faltas = assiduidade
fraca. Horas: menos de 30 = tempo parcial; de 30 a 40, inclusive = tempo
completo; mais de 40 = horas extraordinárias. Apresentar o número total
de funcionários.

  -----------------------------------------------------------------------
  Registos dos funcionários (nome, horas, faltas, Resultado esperado)                      
  ----------------------------------- -----------------------------------
  `Ana, 40, 0; END`                   Ana: Assiduidade perfeita; Tempo
                                      completo. Funcionários: 1

  `Bruno, 25, 1; END`                 Bruno: Boa assiduidade; Tempo
                                      parcial. Funcionários: 1

  `Carla, 45, 3; END`                 Carla: Assiduidade fraca; Horas
                                      extraordinárias. Funcionários: 1

  `Diogo, 30, 2; Eva, 41, 0; END`     Diogo: Boa assiduidade; Tempo
                                      completo. Eva: Assiduidade
                                      perfeita; Horas extraordinárias.
                                      Funcionários: 2

  `END`                               Nenhum registo de funcionário;
                                      Funcionários: 0
  -----------------------------------------------------------------------