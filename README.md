<h1 align="center">
📄<br>Padronizando commits 
</h1>

<h1 align="center">
  <img src="git-commit-img.png">
</h1>

<p>
  O <strong>Convetional Commits</strong> é uma convenção simples de mensagens de commit que segue um conjunto de regras e ajuda os projetos a terem um histórico de commit explícito e bem estruturado
</p>

<p>
  Utilizar estes commits facilitam o entendimento de onde está se concentrando as horas do projeto e a entrada de novos Devs no projeto. Adotando essa convenção, apesar de gastar um pouco mais tempo no código, ajuda a deixar tudo mais organizado e facil de ser entendido.
</p>




## 👾 Convetional Commits

O commit semântico utiliza algumas regras estruturais (listadas abaixo) para facilitar os utilizadores do seu código identificarem as alterações feitas nele.

- `test` - Commits do tipo test indicam qualquer tipo de criação ou alteração de códigos de teste

- `feat`- Commits do tipo feat indicam o desenvolvimento de uma nova feature ao projeto.

- `refactor` - Commits do tipo refactor são utilizados quando ocorre uma refatoração de código que não tenha impacto na lógica/regras de negócio do sistema.

- `style` - Commits do tipo style são utilizados quando há mudanças de formatação e estilo do código que <strong>não alteram</strong> o sistema de forma nenhuma.

- `fix` - Commits do tipo fix são utilizados quando há correção de erros que estão gerando bugs no sistema.

- `chore` - Commits do tipo chore indicam mudanças no projeto que não afetam o sistema ou arquivos de testes. São mudanças de desenvolvimento.

- `docs` - Commits do tipo docs são utilizados quando ocorrem mudanças na documentação da API, mudanças no README, etc.

- `build` - Commits do tipo build indicam mudanças que afetam o processo de build do projeto ou dependências externas.

- `perf` - Commits do tipo perf indicam uma alteração que melhorou a performance do sistema.

- `ci` - Commits do tipo ci é utilizado para mudanças nos arquivos de configuração de CI.

- `revert` - Commits do tipo revert indicam uma reversão do commit anterior.

<strong>Exemplo de uso dos tipos de commit:</strong>
```bash 
git commit -m "style: Adiciona formatação do index"
```

## ⭐️ Recomendações

- Utilize o modo imperativo na mensagem do commit, como <strong>"Adiciona feature"</strong> ao invés de <strong>"Adicionando feature"</strong> ou <strong>"Adicionada feature"</strong>;
- Na primeira linha do seu commit tente usar no máximo 4 palavras;
- Descreva com mais detalhes as alterações feitas no código utilizando o corpo do commit;
- Utilize um emoji no início do commit para ajudar a identifica-lo;
- Faça commits apenas quando as mudanças forem relevantes. Isto é, não faça um commit toda vez que mudar uma linha no código <strong>a menos que seja algo muito especifico e significativo por si só.</strong> O melhor é, se ainda estiver desenvolvendo, espere até que tenha um conjunto importante de alterações para fazer um commit;

## ☄️ Estrutura de um commit
```bash
git commit -m "Descrição (obrigatório)
> [Linha em branco]
> Corpo do Commit (opcional)
> [Linha em branco]
> Footer do commit (opcional)"
```

## 🔮 Personalizando commits com emojis
<p>Uma outra forma de identificar seus commits é por meio de emojis. Apesar de não serem uma forma oficial de padronizar seus commits, emojis podem ser muito uteis para indicar de uma forma rápida e bonita as alterações feitas em seu projeto.</p>
<p>Abaixo segue uma lista com emojis e pra que situações eles podem ser utilizados.</p>

## 💈 Padrões de emojis

<table>
  <thead>
    <tr>
      <th>Tipo de commit</th>
      <th>Emojis</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>Commit inicial</td>
      <td> 🎉 <code>:tada:</code>   </td>
    </tr>
    <tr>
      <td> Atualização de Segurança  </td>
      <td> 🔒 <code>:lock:</code>   </td>
    </tr>
    <tr>
      <td>  Nova feature   </td>
      <td> 🚀 <code>:rocket:</code>   </td>
    </tr>
    <tr>
      <td>  Mudanças na formatação/estilo    </td>
      <td> 🎨 <code> :art: </code>   </td>
    </tr>
    <tr>
      <td>  Correção de bugs  </td>
      <td> 🐛 <code>:bug:</code>   </td>
    </tr>
    <tr>
      <td>  Documentação  </td>
      <td> 📝 <code>:pencil:</code>   </td>
    </tr>
    <tr>
      <td>  Testes  </td>
      <td> 🧪 <code>:test_tube: </code>   </td>
    </tr>
    <tr>
      <td>   Melhorias de Performance        </td>
      <td> 🎚️ <code> :level_slider: </code>   </td>
   </tr>
    <tr>
      <td>  Acessibilidade    </td>
      <td> ♿ <code> :wheelchair: </code>   </td>
    </tr>
    <tr>
      <td>  Apagando arquivos   </td>
      <td> 🗑️ <code> :wastebasket: </code>   </td>
    </tr>
    <tr>
      <td>  Em desenvolvimento        </td>
      <td> 🚧 <code> :construction: </code>   </td>
    </tr>
    <tr>
      <td>   Arquivos de configuração        </td>
      <td> 🧰 <code> :toolbox: </code>   </td>
    </tr>
      <td>   Alterações de revisão de código        </td>
      <td> 👌 <code> :ok_hand: </code>   </td>
    </tr>
   <tr>
      <td>   Nova versão        </td>
      <td> 🎁 <code> :gift: </code>   </td>
   </tr>
    <tr>
      <td>   Mover/Renomear        </td>
      <td> 🚚 <code> :truck: </code>   </td>
    </tr>
  </tbody>
</table>

## 💻 Exemplo do uso de emoji em um commit
```bash
git commit -m ":rocket: Adiciona as classes de acesso ao banco de dados
>
>Adiciona o arquivo Connection.php com a classe para acesso
>ao banco de dados MySQL
>
>Correção do Issue #12"
```

## 💡 Como colocar descrição do commit no terminal
```bash
git commit -m ":rocket: Adiciona as classes de acesso ao banco de dados" -m "Adiciona o arquivo Connection.php com a classe para acesso
ao banco de dados MySQL" -m "Correção do Issue #12"
```

Inspirado no repositório padroes-de-commit de <strong>iuricode</strong><br>
[Clique aqui](https://github.com/iuricode/padroes-de-commits.git) para acessá-lo.

 <!-- <br>[⬆ Voltar ao top](#ideias-de-commit-) <br> -->
