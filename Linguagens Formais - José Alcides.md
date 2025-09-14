---
Disciplina: Linguagens_formais_automatos_finitos
Professor: George
Aluno: José Alcides


### Questões sobre o Processo de Compilação em Java

1. Qual é a principal diferença entre o processo de compilação em Java e o de linguagens C++?:
    A principa diferença de ambos está em como é feito essa compilação, no Java ela passa por um processo intermediario, primeiro ele é convertido para bytecode pelo javac, depois é interpretado ou compilado pela Java Virtual Machine.
    Já o C++ o executável gerado roda diretamente no sistema operacional, sem necessidade de uma máquina virtual.

2. Explique o que acontece em cada uma das três fases de análise do compilador **javac**: Análise Léxica, Análise Sintática e Análise Semântica.
    Na análise léxica, o código-fonte é lido caractere por caractere e transformado em unidades chamadas tokens, que representam elementos como palavras-chave, identificadores, operadores e literais. Essa etapa organiza os símbolos e prepara o terreno para as próximas fases.
    Depois, ocorre a análise sintática, que verifica se esses tokens estão organizados de acordo com as regras gramaticais da linguagem Java. É nessa fase que o compilador identifica estruturas como declarações de variáveis, chamadas de métodos e blocos de controle, construindo uma árvore sintática que representa a hierarquia do código. 
    Ja análise semântica garante que o código faça sentido logicamente. Ela verifica se variáveis foram declaradas antes de serem usadas, se os tipos de dados são compatíveis entre si, se os métodos são chamados corretamente e se as regras de escopo e visibilidade estão sendo respeitadas. Essas três etapas trabalham em conjunto para assegurar que o código esteja correto e pronto para ser transformado em bytecode, permitindo sua execução segura e eficiente pela máquina virtual Java.

3. O que é o **bytecode** e qual é a sua principal função no processo de compilação do Java?:
    O bytecode é o código intermediário gerado pelo compilador Java (javac) a partir do código-fonte. Ele é executado pela Java Virtual Machine (JVM), não diretamente pelo sistema operacional. Sua principal função é garantir a portabilidade, o mesmo bytecode pode rodar em qualquer plataforma que tenha uma JVM, sem precisar recompilar.

4. Qual é o papel da **Máquina Virtual Java (JVM)** na execução de um programa Java, e por que o arquivo ".class" não é executado diretamente pelo sistema operacional?:
    A JVM executa o bytecode gerado pelo compilador Java. Ela interpreta ou compila esse código em tempo real para que funcione no sistema operacional. O arquivo .class não é executado diretamente porque contém bytecode, que não é compreendido pelo sistema — apenas pela JVM. Isso garante que o mesmo programa Java rode em qualquer plataforma com JVM instalada.

5. O que é o compilador **JIT** e como ele melhora o desempenho dos programas em Java?:
    O compilador JIT que significa Just-In-Time é parte da JVM que transforma o bytecode em código de máquina nativo durante a execução do programa. Ele melhora o desempenho ao evitar que o bytecode seja interpretado repetidamente, compilando apenas os trechos mais usados. Isso torna a execução mais rápida e eficiente.

### Questões sobre Linguagens Formais em Java

6. Qual é a aplicação mais comum e direta das linguagens formais em Java, e para que ela é utilizada?:
    As linguagens formais em Java são usadas para definir a gramática da linguagem, permitindo que o compilador reconheça e valide a estrutura do código. Elas são aplicadas principalmente na análise sintática, para verificar se o código está escrito corretamente antes de ser compilado.

7. No processo de compilação de um código Java, como as linguagens formais são usadas nas fases de Análise Léxica e Análise Sintática?:
    No processo de compilação Java, as linguagens formais são usadas na análise léxica para definir os padrões de tokens por meio de expressões regulares, e na análise sintática para definir a estrutura do código usando gramáticas formais. Isso permite que o compilador reconheça e valide a escrita correta do programa.

8. O que é uma **Máquina de Estado Finito (FSM)** e como ela pode ser usada em Java?:
    Uma Máquina de Estado Finito (FSM) é um modelo computacional que representa um sistema com estados definidos e transições entre eles, baseadas em eventos ou entradas.
    Ela pode ser usada para:
    Controlar fluxos de lógica complexa (ex: validação de sequência de caracteres)
    Implementar parsers, protocolos de comunicação ou lógica de jogos
    Usar enums para representar estados e símbolos, e uma tabela de transição (array ou mapa) para definir mudanças de estado.

9. Como as linguagens formais se relacionam com os schemas de validação de documentos, como os usados para **XML** e **JSON**?:
    As linguagens formais são usadas nos schemas de validação de XML e JSON para definir regras sintáticas e estruturais que os documentos devem seguir. Em XML, isso é feito com DTD ou XML Schema, que usam gramáticas formais para validar a estrutura e os tipos de dados. Em JSON, o JSON Schema aplica regras formais para validar propriedades, tipos e formatos dos dados

10. De acordo com o texto, qual é a principal utilidade de ferramentas como o **ANTLR** no contexto de linguagens formais em Java?:

---