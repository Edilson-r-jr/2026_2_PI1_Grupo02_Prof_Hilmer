# Projeto Conceitual do Produto

## Características Gerais

Descreva o produto de forma geral. Apresente os principais conceitos teóricos relacionados ao projeto, que serão aprofundados ou detalhados nas etapas seguintes.

## Estrutura

Apresente o desenho em CAD do produto, indicando:

- Dimensões (lados, arestas e cotas);
- Materiais utilizados;
- Explicação do desenho;
- Justificativa das principais decisões de projeto.

## Descrição de Hardware

A descrição do hardware deve permitir que outras pessoas consigam reproduzir o produto desenvolvido. Para isso, apresente uma descrição dos principais subsistemas e justifique as escolhas de projeto.

Inclua obrigatoriamente:

- **Diagrama de blocos**, apresentando uma visão geral do hardware, seus principais subsistemas e as conexões entre eles.
- **Esquemático elétrico**, mostrando:
  - Componentes utilizados;
  - Símbolos elétricos;
  - Conexões entre os componentes;
  - Pinagem dos dispositivos.

> **Importante:** ligações em protoboard não são consideradas esquemáticos.

A título de exemplo, a Figura abaixo apresenta o diagrama de blocos e o esquemático de um circuito conversor de corrente alternada para corrente direta. Repare que o diagrama de blocos indica os sub-sistemas do circuito completo apresentado no esquemático. 

<figure>

| Diagrama de blocos | Esquemático |
|:------------------:|:-----------:|
| <img src="https://raw.githubusercontent.com/fcte-pi1/template/refs/heads/main/docs/relatorio/figuras/Exemplo-diagrama-de-blocos.png" alt="Diagrama de blocos" width="450"> | <img src="https://raw.githubusercontent.com/fcte-pi1/template/refs/heads/main/docs/relatorio/figuras/Esquematico.png" alt="Esquemático" width="450"> |

<figcaption>

**Figura 1.** Diagrama de blocos e esquemático de um circuito conversor de corrente alternada para corrente contínua. Extraído de GIBILISCO, S. _Beginner´s guide to reading schematics_. McGraw-Hill Education, 2014.

</figcaption>

</figure>

## Análise de Consumo Energético

Apresente os cálculos de consumo energético dos componentes do sistema e justifique as decisões de projeto relacionadas à alimentação elétrica.

### Identificação dos Subsistemas Elétricos

Liste todos os componentes que consomem energia, como:

- Sensores;
- Microcontroladores;
- Atuadores;
- Módulos de comunicação;
- Dispositivos de armazenamento.

Para cada componente informe:

- Tensão de operação (V);
- Corrente média (mA);
- Tempo estimado de utilização (s).

### Cálculo da Energia Consumida

Calcule a energia consumida por cada componente utilizando:

\[
E = V \times I \times t
\]

onde:

- **E** = energia (J);
- **V** = tensão (V);
- **I** = corrente (A);
- **t** = tempo (s).

### Estimativa do Consumo Total

Some a energia consumida por todos os componentes para obter o consumo total do sistema.

### Escolha da Fonte de Alimentação

Converta o consumo para watt-hora (Wh):

> **1 Wh = 3600 J**

Inclua uma margem de segurança adequada e selecione uma bateria ou fonte compatível com a demanda do projeto.

### Planejamento do Circuito de Alimentação

Analise a necessidade de:

- Reguladores de tensão;
- Proteção contra sobrecorrente;
- Isolamento elétrico de atuadores;
- Controle das oscilações de tensão.

### Monitoramento via Software

Implemente rotinas capazes de:

- Medir a tensão da bateria;
- Registrar o tempo de operação;
- Armazenar os dados para análise.

### Validação Experimental

Realize testes reais para comparar o consumo estimado com o consumo medido.

Caso necessário:

- ajuste a fonte de alimentação;
- refine o software de aquisição;
- justifique diferenças entre resultados teóricos e experimentais.

## Descrição de Software

A documentação do software deverá conter, no mínimo, os itens a seguir.

### Diagrama BPMN

Apresente um diagrama BPMN mostrando:

- Atores do sistema;
- Atividades;
- Entradas;
- Saídas.

### Backlog Funcional

Elabore o backlog utilizando:

- Histórias de usuário **ou**
- Casos de uso.

Classifique cada requisito segundo o método **MoSCoW**:

- Must Have;
- Should Have;
- Could Have.

### Backlog Não Funcional

Liste os requisitos não funcionais de forma objetiva.

Exemplo:

> A página deverá carregar em até 5 segundos utilizando conexão 4G.

### Diagrama de Casos de Uso

Apresente:

- Atores;
- Casos de uso;
- Relacionamentos (*include*, *extend*, etc.).

### Arquitetura da Solução

Descreva:

- Objetivo do software;
- Estilo arquitetural adotado;
- Justificativa da arquitetura.

Inclua:

- Padrão arquitetural (MVC, MVP, Microsserviços, Monolítico etc.);
- Linguagens de programação;
- Frameworks e bibliotecas;
- Banco de dados utilizado.

Apresente também um **diagrama de alto nível** contendo:

- Front-end;
- Back-end;
- Componentes;
- Responsabilidades;
- Fluxo de comunicação.

### Persistência de Dados

Apresente o diagrama Entidade-Relacionamento (ER) do banco de dados.

### Análise de Dados

Apresente as principais variáveis do projeto utilizando tabelas, gráficos ou outras representações adequadas.

### Diagrama de Estados

Apresente os estados assumidos pelo software e os eventos responsáveis pelas transições.

### Protótipo

Inclua um protótipo navegável da solução proposta.

### Roteiro de Testes Funcionais

Para cada caso de teste informe:

- Código do caso de teste;
- Nome do caso de teste;
- Tipo (unitário, integração ou sistema);
- Objetivo;
- Pré-condições;
- Procedimento de execução;
- Resultado esperado;
- Correção necessária (caso reprovado);
- Resultado após o reparo.
