# Requisitos

## Requisitos Funcionais

Esta seção descreve os requisitos específicos relacionados às funcionalidades do sistema, como páginas, formulários e validações necessários para a realização das tarefas descritas nos casos de uso.

### Controllers

#### [RF-C01] Mensagens de Erro

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

## Requisitos Não Funcionais