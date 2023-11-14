# Casos de Uso

Os casos de uso são utilizados para especificar as tarefas e os atores envolvidos nelas. Será utilizado futuramente para especificar os requisitos funcionais e não funcionais do projeto.

## Tabela de Conteúdos

[Casos de Uso](#casos-de-uso)

* [UC-01 Realizar Cadastro](#uc-01-realizar-cadastro)
* [UC-02 Realizar Login](#uc-02-realizar-login)
* [UC-03 Visualizar Página Inicial](#uc-03-visualizar-página-inicial)
* [UC-04 Criar Crachás](#uc-04-criar-crachás)
* [UC-05 Visualizar Crachás](#uc-05-visualizar-crachás)
* [UC-06 Modificar Crachás](#uc-06-modificar-crachás)
* [UC-07 Deletar Crachás](#uc-07-deletar-crachás)
* [UC-08 Exportar Crachás](#uc-08-exportar-crachás)

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
    <td><ul>
      <li>Usuário Não Autenticado</li>
      <li>Sistema</li>
    </ul></td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>O caso de uso descreve o processo pelo qual um novo usuário cria uma conta no sistema.</td>
  </tr>
  <tr>
    <th>Fluxo Principal</th>
    <td><ol>
      <li>O novo usuário acessa a página de registro no sistema.</li>
      <li>O sistema exibe o formulário de cadastro.</li>
      <li>O usuário preenche os campos nome, email, senha e aceito os termos de uso. O usuário também pode marcar um checkbox concordando que suas estatísticas de uso sejam compartilhadas com os desenvolvedores.</li>
      <li>O sistema valida as informações fornecidas.</li>
      <li>Se as informações são válidas, o sistema envia um número de para a confirmação de cadastro por e-mail.</li>
      <li>O usuário confirma o cadastro digitando o número enviado por e-mail.</li>
      <li>O sistema confirma o cadastro e registra um novo usuário. Depois redireciona o usuário para a página de login.</li>
    </ol></td>
  </tr>
  <tr>
    <th>Fluxo Alternativo 4-a: Informações Inválidas</th>
    <td><ol>
      <li>Se as informações fornecidas pelo usuário são inválidas, o sistema exibe mensagens de erro correspondentes.</li>
    <ol></td>
  </tr>
  <tr>
    <th>Fluxo Alternativo 8-a: Código de Verificação Incorreto</th>
    <td><ol>
      <li>Se o código de confirmação for inválido, o sistema mostra uma mensagem de erro correspondente.</li>
    <ol></td>
  </tr>
  <tr>
    <th>Pré-Condições</th>
    <td><ul>
      <li>O usuário tem acesso à página de registro.</li>
      <li>O usuário possui um endereço de email válido.</li>
    </ul></td>
  </tr>
  <tr>
    <th>Pós-Condições</th>
    <td><ul>
      <li>Um novo registro de usuário é criado no sistema.</li>
      <li>O usuário recebe um código de confirmação pelo e-mail.</li>
    </ul></td>
  </tr>
  <tr>
    <th>Requisitos Funcionais</th>
    <td><ul>
    </ul></td>
  </tr>
  <tr>
    <th>Requisitos Não Funcionais</th>
    <td><ul>
    </ul></td>
  </tr>
  <tr>
    <th>Casos de Uso Relacionados</th>
    <td><ul>
      <li><a href="#uc-02-realizar-login">[UC-02] Realizar Login</a></li>
    </ul></td>
  </tr>
  <tr>
    <th>Notas</th>
    <td><ul>
      <li>Certificar-se de fornecer feedback claro ao usuário durante o processo de cadastro</li>
    </ul></td>
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
    <td><ul>
      <li>Usuário Não Autenticado</li>
      <li>Sistema</li>
    </ul></td>
  </tr>
  <tr>
    <th>Descrição</th>
    <td>O caso de uso descreve o processo pelo qual um usuário autentica sua identidade para realizar o sistema.</td>
  </tr>
  <tr>
    <th>Fluxo Principal</th>
    <td><ol>
      <li> O usuário acessa a página de login do sistema.</li>
      <li>O sistema exibe um formulário de login.</li>
      <li>O usuário insere suas credenciais (e-mail e senha).</li>
      <li>O sistema valida as informações fornecidas.</li>
      <li>Se as informações são válidas, o sistema concede acesso ao usuário.</li>
      <li>O sistema redireciona o usuário para a página principal.</li>
  </tr>
  <tr>
    <th>Fluxo Alternativo 4-a: Informações Inválidas</th>
    <td><ol>
      <li>Se as credenciais fornecidas pelo usuário são inválidas, o sistema exibe uma mensagem de erro.</li>
    <ol></td>
  </tr>
  <tr>
    <th>Pré-Condições</th>
    <td><ul>
      <li>O usuário possui uma conta registrada no sistema</li>
    </ul></td>
  </tr>
  <tr>
    <th>Pós-Condições</th>
    <td><ul>
      <li>O usuário está autenticado no sistema e pode acessar funcionalidades restritas (salvar os crachás no site).</li>
    </ul></td>
  </tr>
  <tr>
    <th>Requisitos Funcionais</th>
    <td><ul>
    </ul></td>
  </tr>
  <tr>
    <th>Requisitos Não Funcionais</th>
    <td><ul>
    </ul></td>
  </tr>
  <tr>
    <th>Casos de Uso Relacionados</th>
    <td><ul>
      <li><a href="#uc-01-realizar-cadastro">[UC-01] Realizar Cadastro</a></li>
    </ul></td>
  </tr>
  <tr>
    <th>Notas</th>
    <td><ul>
      <li>Implementar medidas de segurança, como bloqueio temporário após múltiplas tentativas de login malsucedidas.</li>
      <li>Oferecer opção de recuperação de senha para usuários esquecidos.</li>
    </ul></td>
  </tr>
</table>

### [UC-03] Visualizar Página Inicial

### [UC-04] Criar Crachás

### [UC-05] Visualizar Crachás

### [UC-06] Modificar Crachás

### [UC-07] Deletar Crachás

### [UC-08] Exportar Crachás
