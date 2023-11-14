# Casos de Uso

Os casos de uso são utilizados para especificar as tarefas e os atores envolvidos nelas. Será utilizado futuramente para especificar os requisitos funcionais e não funcionais do projeto.

## Tabela de Conteúdos

- [Casos de Uso](#casos-de-uso)
  - [UC-01 Realizar Cadastro](#uc-01-realizar-cadastro)
  - [UC-02 Realizar Login](#uc-02-realizar-login)
  - [UC-03 Visualizar Página Inicial](#uc-03-visualizar-página-inicial)
  - [UC-04 Criar Crachás](#uc-04-criar-crachás)
  - [UC-05 Visualizar Crachás](#uc-05-visualizar-crachás)
  - [UC-06 Modificar Crachás](#uc-06-modificar-crachás)
  - [UC-07 Deletar Crachás](#uc-07-deletar-crachás)
  - [UC-08 Exportar Crachás](#uc-08-exportar-crachás)

## Casos de Uso

![Diagrama de Casos de Uso](/Diagramas/Diagrama%20de%20Casos%20de%20Uso.png "Diagrama de Casos de Uso")

### [UC-01] Realizar Cadastro

![Diagrama de Atividades - UC-01](/Diagramas/Diagramas%20de%20Atividades/[UC-01]%20Realizar%20Cadastro.png "Diagrama de Atividades - UC-01")

<table>
  <tr>
    <th>Nome</th>
    <td>Realizar Cadastro</td>
  </tr>
  <tr>
    <th>ID</th>
    <td>UC-01</td>
  </tr>
  <tr>
    <th>Atores</th>
    <td>
      <ul>
        <li>Usuário Não Autenticado</li>
        <li>Sistema</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>O caso de uso descreve o processo pelo qual um novo usuário cria uma conta no sistema.</td>
  </tr>
  <tr>
    <th>Fluxo Principal</th>
    <td>
      <ol>
        <li>O novo usuário acessa a página de registro no sistema.</li>
        <li>O sistema exibe o formulário de cadastro.</li>
        <li>O usuário preenche os campos nome, email, senha e aceito os termos de uso. O usuário também pode marcar um checkbox concordando que suas estatísticas de uso sejam compartilhadas com os desenvolvedores.</li>
        <li>O sistema valida as informações fornecidas.</li>
        <li>Se as informações são válidas, o sistema envia um número de para a confirmação de cadastro por e-mail.</li>
        <li>O usuário confirma o cadastro digitando o número enviado por e-mail.</li>
        <li>O sistema confirma o cadastro e registra um novo usuário. Depois redireciona o usuário para a página de login.</li>
      </ol>
    </td>
  </tr>
  <tr>
    <th>Fluxo Alternativo 4-a: Informações Inválidas</th>
    <td>
      <ol>
        <li>Se as informações fornecidas pelo usuário são inválidas, o sistema exibe mensagens de erro correspondentes.</li>
      <ol>
    </td>
  </tr>
  <tr>
    <th>Fluxo Alternativo 8-a: Código de Verificação Incorreto</th>
    <td>
      <ol>
        <li>Se o código de confirmação for inválido, o sistema mostra uma mensagem de erro correspondente.</li>
      <ol>
    </td>
  </tr>
  <tr>
    <th>Pré-Condições</th>
    <td>
      <ul>
        <li>O usuário tem acesso à página de registro.</li>
        <li>O usuário possui um endereço de email válido.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Pós-Condições</th>
    <td>
      <ul>
        <li>Um novo registro de usuário é criado no sistema.</li>
        <li>O usuário recebe um código de confirmação pelo e-mail.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Requisitos Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Requisitos Não Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Casos de Uso Relacionados</th>
    <td>
      <ul>
        <li><a href="#uc-02-realizar-login">[UC-02] Realizar Login</a></li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Notas</th>
    <td>
      <ul>
        <li>Certificar-se de fornecer feedback claro ao usuário durante o processo de cadastro</li>
      </ul>
    </td>
  </tr>
</table>

### [UC-02] Realizar Login

![Diagrama de Atividades - UC-02](/Diagramas/Diagramas%20de%20Atividades/[UC-02]%20Realizar%20Login.png "Diagrama de Atividades - UC-02")

<table>
  <tr>
    <th>Nome</th>
    <td>Realizar Login</td>
  </tr>
  <tr>
    <th>ID</th>
    <td>UC-02</td>
  </tr>
  <tr>
    <th>Atores</th>
    <td>
      <ul>
        <li>Usuário Não Autenticado</li>
        <li>Sistema</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>O caso de uso descreve o processo pelo qual um usuário autentica sua identidade para realizar o sistema.</td>
  </tr>
  <tr>
    <th>Fluxo Principal</th>
    <td>
      <ol>
        <li> O usuário acessa a página de login do sistema.</li>
        <li>O sistema exibe um formulário de login.</li>
        <li>O usuário insere suas credenciais (e-mail e senha).</li>
        <li>O sistema valida as informações fornecidas.</li>
        <li>Se as informações são válidas, o sistema concede acesso ao usuário.</li>
        <li>O sistema redireciona o usuário para a página principal.</li>
    </tr>
  <tr>
    <th>Fluxo Alternativo 4-a: Informações Inválidas</th>
    <td>
      <ol>
        <li>Se as credenciais fornecidas pelo usuário são inválidas, o sistema exibe uma mensagem de erro.</li>
      <ol>
    </td>
  </tr>
  <tr>
    <th>Pré-Condições</th>
    <td>
      <ul>
        <li>O usuário possui uma conta registrada no sistema</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Pós-Condições</th>
    <td>
      <ul>
        <li>O usuário está autenticado no sistema e pode acessar funcionalidades restritas (salvar os crachás no site).</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Requisitos Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Requisitos Não Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Casos de Uso Relacionados</th>
    <td>
      <ul>
        <li><a href="#uc-01-realizar-cadastro">[UC-01] Realizar Cadastro</a></li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Notas</th>
    <td>
      <ul>
        <li>Implementar medidas de segurança, como bloqueio temporário após múltiplas tentativas de login malsucedidas.</li>
        <li>Oferecer opção de recuperação de senha para usuários esquecidos.</li>
      </ul>
    </td>
  </tr>
</table>

### [UC-03] Visualizar Página Inicial

![Diagrama de Atividades - UC-03](/Diagramas/Diagramas%20de%20Atividades/[UC-03]%20Visualizar%20Página%20Inicial.png "Diagrama de Atividades - UC-03")

<table>
  <tr>
    <th>Nome</th>
    <td>Visualizar Página Inicial</td>
  </tr>
  <tr>
    <th>ID</th>
    <td>UC-03</td>
  </tr>
  <tr>
    <th>Atores</th>
    <td>
      <ul>
        <li>Usuário</li>
        <li>Sistema</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>O caso de uso descreve a interação do usuário com a página inicial do sistema após o login.</td>
  </tr>
  <tr>
    <th>Fluxo Principal</th>
    <td>
      <ol>
        <li>Usuário acessa a página inicial.</li>
        <li>O sistema verifica se o usuário está logado.</li>
        <li>Se o usuário está logado, a página inicial exibe o crachá mais recente do usuário.</li>
      </ol>
  </tr>
  <tr>
    <th>Fluxo Alternativo 4-a: Informações Inválidas</th>
    <td>
      <ol>
        <li>Se o usuário não está logado, o sistema mostra a mensagem “Para salvar os seus crachás, faça login”.</li>
      </ol>
    </td>
  </tr>
  <tr>
    <th>Pré-Condições</th>
    <td>
      <ul>
        <li>O usuário possui uma conta registrada no sistema</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Pós-Condições</th>
    <td>
      <ul>
        <li>O usuário visualiza o conteúdo da página inicial.</li>
        <li>O usuário pode acessar as funcionalidades da aplicação.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Requisitos Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Requisitos Não Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Casos de Uso Relacionados</th>
    <td>
      <ul>
        <li><a href="#uc-02-realizar-login">[UC-02] Realizar Login</a></li>
        <li><a href="#uc-04-criar-crachas">[UC-04] Criar Crachás</a></li>
        <li><a href="#uc-05-visualizar-crachas">[UC-05] Visualizar Crachás</a></li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Notas</th>
    <td>
      <ul>
        <li>Certificar-se de uma navegação intuitiva e fácil acesso a funcionalidades importantes a partir da página inicial.</li>
      </ul>
    </td>
  </tr>
</table>

### [UC-04] Criar Crachás

![Diagrama de Atividades - UC-04](/Diagramas/Diagramas%20de%20Atividades/[UC-04]%20Criar%20Crachás.png "Diagrama de Atividades - UC-04")

<table>
  <tr>
    <th>Nome</th>
    <td>Criar Crachás</td>
  </tr>
  <tr>
    <th>ID</th>
    <td>UC-04</td>
  </tr>
  <tr>
    <th>Atores</th>
    <td>
      <ul>
        <li>Usuário</li>
        <li>Sistema</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>O caso de uso descreve o processo pelo qual o usuário cria um ou mais crachás no sistema.</td>
  </tr>
  <tr>
    <th>Fluxo Principal</th>
    <td>
      <ol>
        <li>O usuário acessa a funcionalidade "Criar Crachás" na página inicial do sistema.</li>
        <li>O sistema exibe um formulário ou interface para a criação de crachás.</li>
        <li>O usuário preenche as informações necessárias para os novos crachás: nome, matrícula, modalidade, curso e foto.</li>
        <li>O sistema valida as informações fornecidas.</li>
        <li>Se as informações são válidas, o sistema cria os crachás.</li>
        <li>O sistema verifica se o usuário está logado.</li>
        <li>Se o usuário está logado, o sistema salva o crachá na conta do usuário.</li>
        <li>O sistema fornece feedback ao usuário sobre a conclusão bem-sucedida do processo.</li>
        <li>O sistema redireciona o usuário para a página de visualização do crachá.</li>
      </ol>
  </tr>
  <tr>
    <th>Fluxo Alternativo 4-a: Informações Inválidas</th>
    <td>
      <ol>
        <li>Se as informações não são validas, o sistema mostra as mensagens de erro correspondentes.</li>
      </ol>
    </td>
  </tr>
  <tr>
    <th>Fluxo Alternativo 6-a: Usuário não está logado</th>
    <td>
      <ol>
        <li>Se o usuário não está logado, o sistema redireciona o usuário para a página de exportar crachás.</li>
      </ol>
    </td>
  </tr>
  <tr>
    <th>Pré-Condições</th>
    <td></td>
  </tr>
  <tr>
    <th>Pós-Condições</th>
    <td>
      <ul>
        <li>O usuário cria um ou mais crachás.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Requisitos Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Requisitos Não Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Casos de Uso Relacionados</th>
    <td>
      <ul>
        <li><a href="#uc-03-visualizar-página-inicial">[UC-03] Visualizar Páginas</a></li>
        <li><a href="#uc-05-visualizar-crachás">[UC-05] Visualizar Crachás</a></li>
        <li><a href="#uc-08-exportar-crachás">[UC-08] Exportar Crachás</a></li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Notas</th>
    <td></td>
  </tr>
</table>

### [UC-05] Visualizar Crachás

![Diagrama de Atividades - UC-05](/Diagramas/Diagramas%20de%20Atividades/[UC-05]%20Visualizar%20Crachás.png "Diagrama de Atividades - UC-05")

<table>
  <tr>
    <th>Nome</th>
    <td>Visualizar Crachás</td>
  </tr>
  <tr>
    <th>ID</th>
    <td>UC-05</td>
  </tr>
  <tr>
    <th>Atores</th>
    <td>
      <ul>
        <li>Usuário Autenticado</li>
        <li>Sistema</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>O caso de uso descreve a interação do usuário com a funcionalidade de visualização dos crachás existentes no sistema.</td>
  </tr>
  <tr>
    <th>Fluxo Principal</th>
    <td>
      <ol>
        <li>O usuário acessa a funcionalidade "Visualizar Crachás" na página inicial.</li>
        <li>O sistema exibe uma lista ou galeria de crachás disponíveis.</li>
        <li>O usuário pode selecionar crachás para realizar as operações: Exportar Crachás, Modificar Crachás e Deletar Crachás, além de criar novos crachás.</li>
      </ol>
  <tr>
    <th>Fluxo Alternativo 2-a: Sem Crachás Disponíveis</th>
    <td>
      <ol>
        <li>Se não houver crachás cadastrados, o sistema exibe uma mensagem indicando a ausência de crachás.</li>
      </ol>
    </td>
  </tr>
  <tr>
    <th>Pré-Condições</th>
    <td>
      <ul>
        <li>O usuário está autenticado no sistema.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Pós-Condições</th>
    <td>
      <ul>
        <li>O usuário visualiza os crachás disponíveis.</li>
        <li>O usuário pode selecionar crachás para realizar outras operações do site.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Requisitos Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Requisitos Não Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Casos de Uso Relacionados</th>
    <td>
      <ul>
        <li><a href="#uc-03-visualizar-página-inicial">[UC-03] Visualizar Página Inicial</a></li>
        <li><a href="#uc-04-criar-crachás">[UC-04] Criar Crachás</a></li>
        <li><a href="#uc-06-modificar-crachás">[UC-06] Modificar Crachás</a></li>
        <li><a href="#uc-07-deletar-crachás">[UC-07] Deletar Crachás</a></li>
        <li><a href="#uc-08-exportar-crachás">[UC-08] Exportar Crachás</a></li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Notas</th>
    <td>
      <ul>
        <li>Implementar uma opção de visualização detalhada para obter informações adicionais sobre cada crachá.</li>
      </ul>
    </td>
  </tr>
</table>

### [UC-06] Modificar Crachás

![Diagrama de Atividades - UC-06](/Diagramas/Diagramas%20de%20Atividades/[UC-06]%20Modificar%20Crachás.png "Diagrama de Atividades - UC-06")

<table>
  <tr>
    <th>Nome</th>
    <td>Modificar Crachás</td>
  </tr>
  <tr>
    <th>ID</th>
    <td>UC-06</td>
  </tr>
  <tr>
    <th>Atores</th>
    <td>
      <ul>
        <li>Usuário Autenticado</li>
        <li>Sistema</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>O caso de uso descreve o processo pelo qual um usuário faz modificações nos crachás existentes no sistema.</td>
  </tr>
  <tr>
    <th>Fluxo Principal</th>
    <td>
      <ol>
        <li>O usuário seleciona os crachás na página de visualizar crachás e seleciona a opção “Modificar Crachás”.</li>
        <li>O sistema exibe um formulário ou interface que permite a edição das informações dos crachás.</li>
        <li>O usuário realiza as modificações desejadas.</li>
        <li>O sistema valida as informações modificadas.</li>
        <li>Se as informações são válidas, o sistema atualiza o crachá com as modificações realizadas.</li>
        <li>O sistema fornece feedback ao usuário sobre a conclusão bem-sucedida do processo.</li>
      </ol>
    </td>
  </tr>
  <tr>
    <th>Fluxo Alternativo 4-a: Informações Inválidas</th>
    <td>
      <ol>
        <li>Se as informações são inválidas, o sistema mostra as mensagens de erro correspondentes.</li>
      </ol>
    </td>
  </tr>
  <tr>
    <th>Pré-Condições</th>
    <td>
      <ul>
        <li>O usuário está autenticado no sistema.</li>
        <li>Existem crachás cadastrados no sistema.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Pós-Condições</th>
    <td>
      <ul>
        <li>O crachá modificado é atualizado no sistema.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Requisitos Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Requisitos Não Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Casos de Uso Relacionados</th>
    <td>
      <ul>
        <li><a href="#uc-05-visualizar-crachás">[UC-05] Visualizar Crachás</a></li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Notas</th>
    <td>
      <ul>
        <li>Oferecer opções de personalização, como atualização de foto ou alteração de informações pessoais.</li>
      </ul>
    </td>
  </tr>
</table>

### [UC-07] Deletar Crachás

![Diagrama de Atividades - UC-07](/Diagramas/Diagramas%20de%20Atividades/[UC-07]%20Deletar%20Crachás.png "Diagrama de Atividades - UC-07")

<table>
  <tr>
    <th>Nome</th>
    <td>Deletar Crachás</td>
  </tr>
  <tr>
    <th>ID</th>
    <td>UC-07</td>
  </tr>
  <tr>
    <th>Atores</th>
    <td>
      <ul>
        <li>Usuário Autenticado</li>
        <li>Sistema</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>O caso de uso descreve o processo pelo qual um usuário exclui crachás existentes no sistema.</td>
  </tr>
  <tr>
    <th>Fluxo Principal</th>
    <td>
      <ol>
        <li>O usuário seleciona os crachás na página de visualizar crachás e seleciona a opção “Deletar Crachás”.</li>
        <li>O sistema solicita confirmação para a exclusão.</li>
        <li>O usuário confirma a exclusão.</li>
        <li>O sistema exclui o crachá do sistema.</li>
        <li>O sistema fornece feedback ao usuário sobre a conclusão bem-sucedida do processo.</li>
      </ol>
    </td>
  </tr>
  <tr>
    <th>Pré-Condições</th>
    <td>
      <ul>
        <li>O usuário está autenticado no sistema.</li>
        <li>Existem crachás cadastrados no sistema.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Pós-Condições</th>
    <td>O crachá é removido do sistema.</td>
  </tr>
  <tr>
    <th>Requisitos Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Requisitos Não Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Casos de Uso Relacionados</th>
    <td>
      <ul>
        <li><a href="#uc-05-visualizar-crachás">[UC-05] Visualizar Crachás</a></li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Notas</th>
    <td>Certificar-se de fornecer uma mensagem de confirmação antes da exclusão para evitar ações acidentais.</td>
  </tr>
</table>

### [UC-08] Exportar Crachás

![Diagrama de Atividades - UC-08](/Diagramas/Diagramas%20de%20Atividades/[UC-08]%20Exportar%20Crachás.png "Diagrama de Atividades - UC-08")

<table>
  <tr>
    <th>Nome</th>
    <td>Exportar Crachás</td>
  </tr>
  <tr>
    <th>ID</th>
    <td>UC-08</td>
  </tr>
  <tr>
    <th>Atores</th>
    <td>
      <ul>
        <li>Usuário</li>
        <li>Sistema</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>O caso de uso "Exportar Crachás" descreve o processo pelo qual um usuário exporta crachás do sistema para pdf ou png.</td>
  </tr>
  <tr>
    <th>Fluxo Principal</th>
    <td>
      <ol>
        <li>O usuário acessa a funcionalidade "Exportar Crachás" no sistema.</li>
        <li>O sistema exibe opções de formatos de exportação, como PDF e PNG.</li>
        <li>O usuário seleciona o formato desejado para exportação.</li>
        <li>O sistema gera um arquivo de exportação contendo as informações dos crachás no formato escolhido.</li>
        <li>O sistema disponibiliza o arquivo para download pelo usuário.</li>
        <li>O sistema fornece feedback ao usuário sobre a conclusão bem-sucedida do processo.</li>
      </ol>
    </td>
  </tr>
  <tr>
    <th>Pré-Condições</th>
    <td>O usuário tem que ter, polo menos, um crachá criado.</td>
  </tr>
  <tr>
    <th>Pós-Condições</th>
    <td>O usuário obtém um arquivo exportado contendo as informações dos crachás.</td>
  </tr>
  <tr>
    <th>Requisitos Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Requisitos Não Funcionais</th>
    <td></td>
  </tr>
  <tr>
    <th>Casos de Uso Relacionados</th>
    <td>
      <ul>
        <li><a href="#uc-04-criar-crachás">[UC-04] Criar Crachás</a></li>
        <li><a href="#uc-05-visualizar-crachás">[UC-05] Visualizar Crachás</a></li>
      </ul>
    </td>
  </tr>
  <tr>
    <th>Notas</th>
    <td>Fornecer informações claras sobre o conteúdo incluído no arquivo de exportação.</td>
  </tr>
</table>