# Requisitos

Esta seção descreve os requisitos funcionais e não funcionais definidos a partir da análise dos casos de uso.

## Tabela de Conteúdos

* Requisitos Funcionais
   * Controllers
      * [[RF-C01] Mensagens de Erro](#rf-c01-mensagens-de-erro)
      * [[RF-C02] Feedback de Cadastro Bem-Sucedido](#rf-c02-feedback-de-cadastro-bem-sucedido)
      * [[RF-C03] Feedback de Crachá Criado Com Sucesso](#rf-c03-feedback-de-crachá-criado-com-sucesso)
      * [[RF-C04] Feedback de Modificação Bem-Sucedida](#rf-c04-feedback-de-modificação-bem-sucedida)
      * [[RF-C05] Feedback de Exclusão Bem-Sucedida](#rf-c05-feedback-de-exclusão-bem-sucedida)
      * [[RF-C06] Feedback de Crachá Exportado Com Sucesso](#rf-c06-feedback-de-crachá-exportado-com-sucesso)
   * Middlewares
      * [[RF-M01] Validar Login](#rf-m01-validar-login)
      * [[RF-M02] Verificar Logado](#rf-m02-verificar-logado)
   * Views
      * [[RF-V01] Página de Cadastro](#rf-v01-página-de-cadastro)
      * [[RF-V02] Formulário de Cadastro](#rf-v02-formulário-de-cadastro)
      * [[RF-V03] Termos e Condições](#rf-v03-termos-e-condições)
      * [[RF-V04] Estatísticas de Uso](#rf-v04-estatísticas-de-uso)
      * [[RF-V05] Página de Login](#rf-v05-página-de-login)
      * [[RF-V06] Formulário de Login](#rf-v06-formulário-de-login)
      * [[RF-V07] Página Inicial](#rf-v07-página-inicial)
      * [[RF-V08] Página de Criação de Crachás](#rf-v08-página-de-criação-de-crachás)
      * [[RF-V09] Formulário para Criação de Crachás](#rf-v09-formulário-para-criação-de-crachás)
      * [[RF-V10] Página de Visualizar Crachás](#rf-v10-página-de-visualizar-crachás)
      * [[RF-V11] Página de Modificar Crachás](#rf-v11-página-de-modificar-crachás)
      * [[RF-V12] Formulário de Modificar Crachás](#rf-v12-formulário-de-modificar-crachás)
      * [[RF-V13] Página de Exportar Crachás](#rf-v13-página-de-exportar-crachás)
      * [[RF-V14] Formulários das Especificações de Exportação](#rf-v14-formulários-das-especificações-de-exportação)
   * Services
      * [[RF-S01] Confirmação do E-mail](#rf-s01-confirmação-do-e-mail)
      * [[RF-S02] Armazenamento das Informações](#rf-s02-armazenamento-das-informações)
      * [[RF-S03] Inserir Crachás](#rf-s03-inserir-crachás)
      * [[RF-S04] Pegar Crachás](#rf-s04-pegar-crachás)
      * [[RF-S05] Atualizar Crachás](#rf-s05-atualizar-crachás)
      * [[RF-S06] Excluir Crachás](#rf-s06-excluir-crachás)
   * Utils
      * [[RF-U01] Criar Crachás](#rf-u01-criar-crachás)
      * [[RF-U02] Validação de Dados de Cadastro](#rf-u02-validação-de-dados-de-cadastro)
      * [[RF-U03] Validação de Dados de Login](#rf-u03-validação-de-dados-de-login)
      * [[RF-U04] Validar Dados dos Crachás](#rf-u04-validar-dados-dos-crachás)
      * [[RF-U05] Selecionar Crachás](#rf-u05-selecionar-crachás)
      * [[RF-U06] Confirmar Exclusão](#rf-u06-confirmar-exclusão)
      * [[RF-U07] Exportar Crachás para PDF](#rf-u07-exportar-crachás-para-pdf)
      * [[RF-U08] Exportar Crachás para PNG](#rf-u08-exportar-crachás-para-png)
      * [[RF-U09] Download dos Crachás](#rf-u09-download-dos-crachás)
* Requisitos Não Funcionais  
   * Safety  
      * [[RNF-S01] Limite de Tentativas de Senha](#rnf-s01-limite-de-tentativas-de-senha)
      * [[RNF-S02] Validação de Email](#rnf-s02-validação-de-email)
      * [[RNF-S03] Limite de Tentativas de Validação de Email](#rnf-s03-limite-de-tentativas-de-validação-de-email)
      * [[RNF-S04] Segurança de Senhas](#rnf-s04-segurança-de-senhas)
   * Product Ethics
      * [[RNF-P01] Valor dos Produtos](#rnf-p01-valor-dos-produtos)
   * Accessibility
      * [[RNF-A01] Responsividade](#rnf-a01-responsividade)
      * [[RNF-A02] Interface Simplificada](#rnf-a02-interface-simplificada)

## Requisitos Funcionais

Esta seção descreve os requisitos específicos relacionados às funcionalidades do sistema, como páginas, formulários e validações necessários para a realização das tarefas descritas nos casos de uso.

### Controllers

#### [[RF-C01] Mensagens de Erro](#tabela-de-conteudos)

<table>
   <tr>
      <th>Nome</th>
      <td>Mensagens de Erro</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-C01</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer feedback claro e de fácil entendimento nos casos de erros como dados inválidos, erro no banco de dados, timeout, etc.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>O sistema deve fornecer feedback claro e de fácil entendimento nos casos de erros como dados inválidos, erro no banco de dados, timeout, etc.</td>
   </tr>
</table>

#### [RF-C02] Feedback de Cadastro Bem-Sucedido

<table>
   <tr>
      <th>Nome</th>
      <td>Feedback de Cadastro Bem-Sucedido</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-C02</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer um feedback, sendo uma página ou um alerta de que o cadastro foi realizado com sucesso.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-C03] Feedback de Crachá Criado Com Sucesso

<table>
   <tr>
      <th>Nome</th>
      <td>Feedback de Crachá criado com sucesso</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-C03</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer um feedback, sendo uma página ou um alerta de que os crachás foram criados com sucesso.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-C04] Feedback de Modificação bem sucedida

<table>
   <tr>
      <th>Nome</th>
      <td> Feedback de Modificação bem sucedida </td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-C04</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer um feedback, sendo uma página ou um alerta de que os crachás foram modificados com sucesso.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-C05] Feedback de Exclusão bem sucedida

<table>
   <tr>
      <th>Nome</th>
      <td> Feedback de Exclusão bem sucedida </td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-C05</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer um feedback, sendo uma página ou um alerta de que os crachás foram excluídos com sucesso.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-C06] Feedback de Crachá exportado com sucesso

<table>
   <tr>
      <th>Nome</th>
      <td> Feedback de Crachá exportado com sucesso </td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-C06</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer um feedback, sendo uma página ou um alerta de que os crachás foram esportados com sucesso.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

### Middlewares

#### [RF-M01] Validar Login

<table>
   <tr>
      <th>Nome</th>
      <td>Validar Login</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-M01</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema verifica os dados do usuário para aprovar ou rejeitar a solicitação de login.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-M02] Verificar Logado

<table>
   <tr>
      <th>Nome</th>
      <td>Verificar Logado</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-M02</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema verifica se o usuário está logado e realiza a permissão ou bloqueio do acesso à página</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

### Views

#### [RF-V01] Página de Cadastro

<table>
   <tr>
      <th>Nome</th>
      <td>Página de Cadastro</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V01</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer uma página de cadastro acessível a partir da página inicial.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-V02] Formulário de Cadastro

<table>
   <tr>
      <th>Nome</th>
      <td>Formulário de Cadastro</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V02</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer um formulário de cadastro com todas as informações necessárias para a criação de sua conta.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>As informações que serão apresentadas no formulário são:
         <ul>
            <li>Nome</li>
            <li>E-mail</li>
            <li>Senha</li>
            <li>Aceitar os Termos de Uso</li>
            <li>Compartilhar as Estatísticas de Uso</li>
         </ul>
      </td>
   </tr>
</table>

#### [RF-V03] Termos e Condições

<table>
   <tr>
      <th>Nome</th>
      <td>Termos e Condições</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V03</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer uma página e um link de acesso que permita ao usuário ler os termos de uso do sistema.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-V04] Estatísticas de Uso

<table>
   <tr>
      <th>Nome</th>
      <td>Estatísticas de Uso</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V04</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer uma página e um link de acesso que permita ao usuário ler as informações do compartilhamento de estatísticas de uso</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-V05] Página de Login

<table>
   <tr>
      <th>Nome</th>
      <td>Página de Login</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V05</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer uma página de login acessível a partir da página inicial.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-V06] Formulário de Login

<table>
   <tr>
      <th>Nome</th>
      <td>Formulário de Login</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V06</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer um formulário de login com todas as informações necessárias para a criação de sua conta.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>As informações que serão apresentadas no formulário são:
         <ul>
            <li>E-mail</li>
            <li>Senha</li>
         </ul>
      </td>
   </tr>
</table>

#### [RF-V07] Página Inicial

<table>
   <tr>
      <th>Nome</th>
      <td>Página Inicial</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V07</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema fornece uma página inicial da qual pode acessar todas as funções do sistema.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>Tanto usuários logados quanto não-logados podem acessar esta página. Se o usuário estiver logado, o crachá criado mais recentemente é mostrado na tela inicial</td>
   </tr>
</table>

#### [RF-V08] Página de Criação de Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Página de Criação de Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V08</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema fornece uma página inicial na qual o usuário pode criar crachás no sistema.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>Tanto usuários logados quanto não-logados podem acessar esta página.</td>
   </tr>
</table>

#### [RF-V09] Formulário para Criação de Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Formulário para Criação de Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V09</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer um formulário de cadastro com todas as informações necessárias para a criação de um ou mais crachás.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>As informações que serão apresentadas no formulário são:
         <ul>
            <li>Nome</li>
            <li>Matrícula</li>
            <li>Tipo</li>
            <li>Curso</li>
            <li>Foto (Opcional)</li>
         </ul>
      </td>
   </tr>
</table>

#### [RF-V10] Página de Visualizar Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Página de Visualizar Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V10</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema fornece uma página na qual o usuário pode ver todos os crachás criados por ele. Ele também pode selecionar crachás para realizar operações como exportar, modificar e deletar.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>Apenas usuários logados podem acessar esta página</td>
   </tr>
</table>

#### [RF-V11] Página de Modificar Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Página de Modificar Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V11</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema fornece uma página na qual o usuário pode modificar um ou mais crachás criados por ele.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>
        Apenas usuários logados podem acessar esta página.
      </td>
   </tr>
</table>

#### [RF-V12] Formulário de Modificar Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Formulário de Modificar Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V12</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer um formulário com todas as informações necessárias para a modificação de um ou mais crachás.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>As informações que serão apresentadas no formulário são:
         <ul>
            <li>Nome</li>
            <li>Matrícula</li>
            <li>Tipo</li>
            <li>Curso</li>
            <li>Foto (Opcional)</li>
         </ul>
      </td>
   </tr>
</table>

#### [RF-V13] Página de Exportar Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Página de Exportar Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V13</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema fornece uma página na qual o usuário pode exportar um ou mais crachás criados por ele.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>
        Tanto usuários logados quanto não-logados podem acessar esta página.
      </td>
   </tr>
</table>

#### [RF-V14] Formulários das Especificações de Exportação

<table>
   <tr>
      <th>Nome</th>
      <td>Formulários das Especificações de Exportação</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-V14</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve fornecer um formulário com todas as informações necessárias para a exportação de um ou mais crachás.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>As informações que serão apresentadas no formulário são:
         <ul>
            <li>Tipo de Arquivo a ser Exportado</li>
         </ul>
      </td>
   </tr>
</table>

### Services

#### [RF-S01] Confirmação do E-mail

<table>
   <tr>
      <th>Nome</th>
      <td>Confirmação do E-mail</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-S01</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema envia um código de confirmação para o e-mail do usuário, o qual deve digitá-lo corretamente para executar o cadastro.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>O código enviado é um código numérico composto por 6 caracteres. O código expira após 10 minutos</td>
   </tr>
</table>

#### [RF-S02] Armazenamento das Informações

<table>
   <tr>
      <th>Nome</th>
      <td>Armazenamento das Informações</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-S02</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve se conectar com o banco de dados para armazenar as informações dos usuários</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-S03] Inserir Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Inserir Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-S03</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema usa os dados inseridos na página criar crachás para gerar e inserir os crachás no banco de dados</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-S04] Pegar Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Pegar Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-S04</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema pega os crachás criados pelo usuário no banco de dados</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-S05] Atualizar Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Atualizar Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-S05</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema atualiza os crachás criados pelo usuário no banco de dados</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-S06] Excluir Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Excluir Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-S06</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema excluí os crachás criados pelo usuário no banco de dados</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

### Utils

#### [RF-U01] Criar Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Criar Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-U01</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>Função que recebe uma array de dados e retorna uma array de crachás.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>As informações que serão utilizadas para a criação dos crachás são:
         <ul>
            <li>Nome</li>
            <li>Matrícula</li>
            <li>Tipo</li>
            <li>Curso</li>
            <li>Foto (Opcional)</li>
         </ul>
      </td>
   </tr>
</table>

#### [RF-U02] Validação de Dados de Cadastro

<table>
   <tr>
      <th>Nome</th>
      <td>Validação de Dados</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-U02</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve verificar os dados fornecidos antes de enviar a solicitação de cadastro para assegurar a integridade dos mesmos.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>As verificações a serem realizadas são:
         <ul>
            <li>Nome : obrigatório</li>
            <li>Email : obrigatório | estrutura de email ‘local@domain.com’</li>
            <li>Senha : obrigatório | mínimo de 6 caracteres, com números, letras maiúsculas e minúsculas e um caractere especial</li>
            <li>Aceitar Termos de Uso : obrigatório</li>
            <li>Compartilhar as Estatísticas de Uso : nenhum</li>
         </ul>
      </td>
   </tr>
</table>

#### [RF-U03] Validação de Dados de Login

<table>
   <tr>
      <th>Nome</th>
      <td>Validação de Login</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-U03</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve verificar os dados fornecidos antes de enviar a solicitação de login para assegurar a integridade dos mesmos.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>A verificação que será realizada é:
         <ul>
            <li>E-mail : obrigatório | estrutura de email ‘local@domain.com’</li>
            <li>Senha : obrigatório</li>
         </ul>
      </td>
   </tr>
</table>

#### [RF-U04] Validar Dados dos Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Validar Dados dos Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-U04</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema deve verificar os dados fornecidos antes de enviar a solicitação de criação do crachá para assegurar a integridade dos mesmos.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>A verificação que será realizada é:
         <ul>
            <li>Nome : obrigatório</li>
            <li>Matrícula : obrigatório | 11 caracteres numéricos</li>
            <li>Tipo : obrigatório | Técnico || Superior</li>
            <li>Curso : obrigatório | estar dentro da lista de cursos respectiva</li>
            <li>Foto : imagem em png, jpg ou webp</li>
         </ul>
      </td>
   </tr>
</table>

#### [RF-U05] Selecionar Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Selecionar Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-U05</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O usuário pode selecionar crachás para realizar operações como exportar, modificar e deletar.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td></td>
   </tr>
</table>

#### [RF-U06] Confirmar Exclusão

<table>
   <tr>
      <th>Nome</th>
      <td>Confirmar Exclusão</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-U06</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O Sistema deve reiterar ao usuário se o mesmo quer realmente excluir um ou mais crachás, dando-lhe a opção de sim ou de não, para poder deletar ou não o/os crachá/ás selecionado/os.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td> 
        Em caso de confirmação da exclusão, deverá ser retornado uma String dizendo: "A exclusão foi realizada com sucesso."
        Em caso de cancelamento da exclusão, o usuário deverá ser redirecionado a página de "Seleção de Crachás"
      </td>
   </tr>
</table>

#### [RF-U07] Exportar Crachás para PDF

<table>
   <tr>
      <th>Nome</th>
      <td>Exportar Crachás para PDF</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-U07</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O Sistema deve converter o/os crachá/ás para o tipo de arquivo PDF, permitindo o usuário o/os exportar para o meio que preferir.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td> 
      Em caso de confirmação da exportação, deverá ser retornado uma String dizendo: "A exportação por PDF foi feita com sucesso!"
      </td>
   </tr>
</table>

#### [RF-U08] Exportar Crachás para PNG

<table>
   <tr>
      <th>Nome</th>
      <td>Exportar Crachás para PNG</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-U08</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O Sistema deve converter o/os crachá/ás para o tipo de arquivo PNG, permitindo o usuário o/os exportar para o meio que preferir.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td> 
      Em caso de confirmação da exportação, deverá ser retornado uma String dizendo: "A exportação por PNG foi feita com sucesso!"
      </td>
   </tr>
</table>

#### [RF-U09] Download dos Crachás

<table>
   <tr>
      <th>Nome</th>
      <td>Download dos Crachás</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RF-U09</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O Sistema deve disponibilizar o/os crachá/ás para download, permitindo o usuário o/os baixar no tipo de arquivo que preferir.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td> 
      Em caso de confirmação do Download, deverá ser retornado uma String dizendo: "Seu Download foi concluído!"
      </td>
   </tr>
</table>

## Requisitos Não Funcionais

Esta seção descreve os requisitos específicos relacionados à como as funcionalidades do sistema serão entregues ao usuário, podendo variar entre tópicos como: usabilidade, confiabilidade, segurança, acessibilidade, ética do produto e etc.

### Safety

#### [RNF-S01] Limite de Tentativas de Senha

<table>
   <tr>
      <th>Nome</th>
      <td>Limite de Tentativas de Senha</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RNF-S01</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O Usuário terá por padrão um máximo de 3 tentativas consecutivas de Login, onde caso o mesmo erre sua senha em um número maior do que o limite estipulado, o sistema acionará sua iniciativa de defesa, dando-lhe um Time-Out curto.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td> 
      Uma String deverá ser retornada ao usuário informando: "Por questões de segurança você deve esperar o tempo estipulado para poder prosseguir com seu Login."
      O Tempo de Time-Out é de: 3 minutos, 11 segundos e 4 décimos.
      </td>
   </tr>
</table>

#### [RNF-S02] Validação de Email

<table>
   <tr>
      <th>Nome</th>
      <td>Validação de Email</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RNF-S02</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O sistema exigirá um código de confirmação de 6 digitos ao usuário buscando a validação de seu endereço digital, o código será enviado por Email e ficará disponível para validação por 10 minutos.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td> 
      </td>
   </tr>
</table>

#### [RNF-S03] Limite de Tentativas de Validação de Email

<table>
   <tr>
      <th>Nome</th>
      <td>Limite de Tentativas de Validação de Email</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RNF-S03</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Usuário</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O Usuário terá por padrão um máximo de 3 tentativas consecutivas de validação de seu email, onde caso o mesmo não valide seu endereço eletrônico em um número de tentativas maior do que o limite estipulado, o sistema acionará sua iniciativa de defesa, dando-lhe um Time-Out curto.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td> 
      Uma String deverá ser retornada ao usuário informando: "Por questões de segurança você deve esperar o tempo estipulado para poder prosseguir com a validação de seu Email."
      O Tempo de Time-Out é de: 3 minutos, 11 segundos e 4 décimos.
      </td>
   </tr>
</table>

#### [RNF-S04] Segurança de Senhas

<table>
   <tr>
      <th>Nome</th>
      <td>Segurança de Senhas</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RNF-S04</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td>O Sistema deverá armazenar as senhas de usuários de forma criptografada para evitar futuros vazamentos ou invasão à privacidade do Usuário.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>
      </td>
   </tr>
</table>

### Product Ethics

#### [RNF-P01] Valor dos Produtos

<table>
   <tr>
      <th>Nome</th>
      <td>Valor dos Produtos</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RNF-P01</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td> As funcionalidades de sistema implementados pela equipe devem ter valor, ou seja, devem ser testadas e aprovadas antes de serem colocadas em produção com o intuito de agregar valor ao produto, ou seja, dar-lhe uma maior credibilidade.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>
      </td>
   </tr>
</table>

### Accessibility

#### [RNF-A01] Responsividade

<table>
   <tr>
      <th>Nome</th>
      <td>Responsividade</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RNF-A01</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td> O Sistema deve apresentar uma interface que consiga se adequar a diferentes tamanhos de telas de diversos dispositivos buscando atender a usuários que utilizem tanto PC quanto o Celular como fontes de acesso.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>
        O modelo Mobile First deve ser o conceito utilizado como referência na implementação da responsividade diante da interface visto que, o mesmo além de representar o foco do público do projeto ainda traz uma série de vantagens de desenvolvimento.
      </td>
   </tr>
</table>

#### [RNF-A02] Interface Simplificada

<table>
   <tr>
      <th>Nome</th>
      <td>Interface Simplificada</td>
   </tr>
   <tr>
      <th>ID</th>
      <td>RNF-A02</td>
   </tr>
   <tr>
      <th>Ator Relacionado</th>
      <td>Sistema</td>
   </tr>
   <tr>
      <th>Descrição</th>
      <td> O Sistema deve apresentar uma interface de fácil uso e acesso, visando a simplicidade em sua utilização, evitando confudir ou tirar o foco do usuário daquilo que o mesmo deveria fazer dentro da aplicação.</td>
   </tr>
   <tr>
      <th>Observações/ Notas Adicionais</th>
      <td>
        Os princípios de Design de Donald Norman devem ser levados em consideração na implementação desse requisito.
      </td>
   </tr>
</table>





