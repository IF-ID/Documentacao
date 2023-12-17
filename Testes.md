# Testes

Os testes são utilizados para trazer um aumento na simplicidade, segurança e produtividade do projeto. Aqui, serão listados os seus diferentes tipos utilizados em seu desenvolvimento e as vantagens de sua utilização perante o código e a interface.

## Tabela de Conteúdos

- [Testes de Aceitação](#testes-de-aceitação)
  - [Heurísticas de Nielsen](#heurísticas-de-nielsen)
    - [[HN-01] Visibilidade do Status do Sistema](#hn-01-visibilidade-do-status-do-sistema)
    - [[HN-02] Compatibilidade entre o sistema e o mundo real](#hn-02-compatibilidade-entre-o-sistema-e-o-mundo-real)
    - [[HN-03] Consistência e Padronização](#hn-03-consistência-e-padronização)
    - [[HN-04] Prevenção de erros](#hn-04-prevenção-de-erros)
    - [[HN-05] Reconhecimento em vez de memorização](#hn-05-reconhecimento-em-vez-de-memorização)
    - [[HN-06] Eficiência e flexibilidade de uso](#hn-06-eficiência-e-flexibilidade-de-uso)
    - [[HN-07] Estética e design minimalista](#hn-07-estética-e-design-minimalista)
    - [[HN-08] Ajude os usuários a reconhecerem, diagnosticarem e recuperarem-se de erros](#hn-08-ajude-os-usuários-a-reconhecerem-diagnosticarem-e-recuperarem-se-de-erros)
- [Test Driven Development (TDD)](#test-driven-development-tdd)
  - [Testes Unitários](#testes-unitários)
  - [Testes de Integração](#testes-de-integração)
  - [Testes de Sistema](#testes-de-sistema)

# [Testes de Aceitação](#tabela-de-conteúdos)

Os testes de aceitação são uma prática comum no desenvolvimento de software que são responsáveis por verificarem se um sistema atende aos requisitos que foram definidos previamente. Sua funcionalidade concentra-se na validação da interface do usuário (UI) e, muitas vezes, envolve a execução de casos de teste que simulam as interações reais do usuário com o sistema.

No caso do IFID, por conta do curto período de tempo, a abordagem escolhida para a realização dos testes de aceitação foi: a prototipação e codificação baseando os resultados da experiência de uso de acordo com as Heurísticas de Nielsen.

As vantagens da utilização de testes de aceitação são diversas, tais como: aprimorar a validação de requisitos do projeto, identificação de problemas de usabilidade, contribuição para a garantia de qualidade e entre diversos outros.


# [Heurísticas de Nielsen](#tabela-de-conteúdos)

As heurísticas de Nielsen são um conjunto de 10 princípios de usabilidade estabelecidos por Jakob Nielsen, um renomado especialista em usabilidade. Essas heurísticas fornecem diretrizes práticas para avaliar a interface do usuário de sistemas interativos. São uma forma de avaliar o design de interface, identificando falhas e erros para corrigi-los e otimizar a UX, ou experiência do usuário.

O motivo de sua escolha como ponto pricipal dos testes de aceitação deriva de sua facilidade de aplicação e identificação de problemas, foco nas necessidades do usuário e aplicabilidade universal. A seguir, as heurísticas de nielsen que a IFID obedece:

### [[HN-01] Visibilidade do Status do Sistema](#tabela-de-conteúdos)

Como diz o nome, a primeira Heurística de Nielsen se baseia em manter o usuário ciente sobre as ações exercidas por si dentro do sistema. Isso ocorre por meio de muitas maneiras, desde uma mensagem pequena de feedback, até uma barra de progresso que demonstra aonde a ação do usuário o levou. 

Dentro do IFID, mensagens de feedback de criação, alteração e exclusão de crachá são um exemplo da primeira heurística, reduzindo a incerteza do usuário quanto a suas ações e reforçando aos mesmos o estado do sistema.

### [[HN-02] Compatibilidade entre o sistema e o mundo real](#tabela-de-conteúdos)

### [[HN-03] Consistência e Padronização](#tabela-de-conteúdos)

### [[HN-04] Prevenção de erros](#tabela-de-conteúdos)

### [[HN-05] Reconhecimento em vez de memorização](#tabela-de-conteúdos)

### [[HN-06] Eficiência e flexibilidade de uso](#tabela-de-conteúdos)

### [[HN-07] Estética e design minimalista](#tabela-de-conteúdos)

### [[HN-08] Ajude os usuários a reconhecerem, diagnosticarem e recuperarem-se de erros](#tabela-de-conteúdos)

# [Test Driven Development (TDD)](#tabela-de-conteúdos)

Test Driven Development (TDD) ou Desenvolvimento Orientado à Testes, refere-se à uma abordagem de desenvolvimento de software que enfatiza a criação de testes automatizados antes da implementação de um código funcional. O processo segue um ciclo de três etapas: escrever um teste, implementar o código mínimo para passar no teste e, em seguida, refatorar o código conforme necessário.

As vantagens referentes à produtividade do desenvolvedor, maior segurança na correção de bugs e no refatoramento, simplicidade de código e melhor feedback de funcionamento, foram fatores cruciais para a escolha do TDD como método de desenvolvimento. No desenvolvimento do IFID, utilizamos 3 diferentes tipos de testes para confirmar o valor do produto, a seguir: os tipos de testes utilizados no desenvolvimento do projeto.

### [Testes Unitários](#tabela-de-conteúdos)

Testes unitários são uma prática de teste de software em que unidades individuais de código, como funções, métodos ou classes, são testadas isoladamente para garantir que funcionem conforme o esperado. O objetivo dos testes unitários é validar que cada parte do código (unidade) opera corretamente, proporcionando confiança de que as unidades, quando combinadas, funcionarão corretamente como um todo.

A razão da utilização de testes unitários durante o desenvolvimento do projeto foram diversas, mas entre elas destacam-se: a facilidade de refatoração e identificação de defeitos, melhoria da qualidade do código e maior organização de código.

### [Testes de Integração](#tabela-de-conteúdos)

Testes de integração são uma prática de teste de software que visa verificar se diferentes módulos ou componentes de um sistema interagem entre si de maneira adequada. O objetivo principal é identificar problemas que podem surgir quando unidades individuais são combinadas para formar um sistema completo. Esses testes garantem que os diversos componentes integrados funcionem corretamente em conjunto.

A razão da utilização de testes de integração durante o desenvolvimento do projeto foram diversas, mas entre elas destacam-se: melhoria na qualidade do software, garantia de fluxo de dados adequados e maior facilidade de identificação de conflitos entre componentes.

### [Testes de Sistema](#tabela-de-conteúdos)

Os testes de sistema são uma fase crítica do ciclo de vida do desenvolvimento de software, focados em avaliar o sistema como um todo para garantir que ele atenda aos requisitos especificados. Esses testes são realizados após os testes unitários e de integração e antes do lançamento do software. O objetivo é verificar se o sistema está pronto para ser implantado e se ele opera conforme o esperado em um ambiente comercial.

A razão da utilização de testes de sistema durante o desenvolvimento do projeto foram diversas, mas entre elas destacam-se: prevenção de possíveis problemas pós lançamento, maior validação da segurança do sistema e definição de desempenho e escalabilidade.
