<a href=""><img src="https://github.com/user-attachments/assets/7a38b221-ab20-4f6d-b409-b52c37104889"></a>

> ⚗️💧 **Preparação**: Para este conteúdo, o aluno deverá dispor de um computador com acesso à internet, um web browser com suporte a HTML 5 (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari, Opera etc.), um editor de texto ou IDE (VSCode etc.) e o software Elixir, com a versão mais recente, instalado na sua máquina local.

# It's a repository of Elixir programming ⚗️💧
<a href="https://elixir-lang.org/install.html"><img src="https://github.com/user-attachments/assets/2ca6c1e3-557d-42ab-8a84-3ed8a8a2ad29" align="right" height="77"></a>

O **Elixir** é uma linguagem de programação dinâmica e funcional, concorrente e de propósito geral, projetada para criar aplicações escaláveis e de alta disponibilidade. Ela roda sobre a máquina virtual do Erlang (BEAM), herdando sua robustez e desempenho para sistemas distribuídos, tolerantes a falhas e com forte suporte à concorrência. Elixir é uma linguagem projetada para ser produtiva, com uma sintaxe elegante e moderna, enquanto aproveita a robustez e os recursos de simultaneidade da máquina virtual Erlang.

Criada por José Valim, um desenvolvedor brasileiro e um dos principais contribuidores do framework Ruby on Rails, Elixir surgiu com o objetivo de combinar a solidez da plataforma Erlang — que é usada em sistemas de telecomunicação com tempo de atividade crítico — com uma sintaxe moderna e produtiva, inspirada em linguagens como Ruby. Ele foi criado para ser escalável e manter sistemas de alta disponibilidade, tornando-o uma escolha popular para aplicativos da Web, sistemas distribuídos e telecomunicações. Elixir combina o melhor dos dois mundos: a simplicidade do Ruby e o poder do Erlang.

Por que usar o Elixir? O foco do Elixir está em aplicações que exigem alta performance e muitos processos simultâneos, como sistemas financeiros, plataformas de mensagens em tempo real, aplicações IoT, e serviços web escaláveis. Seu modelo funcional evita efeitos colaterais e facilita a manutenção do código, enquanto sua estrutura baseada em processos leves permite criar sistemas que lidam com milhões de conexões simultâneas. 

- **Simultaneidade**: O Elixir facilita a escrita de código simultâneo, aproveitando os processos leves do BEAM.
- **Escalabilidade**: Ideal para aplicativos que precisam lidar com um grande número de conexões simultâneas.
- **Alta disponibilidade**: Projetado para sistemas que precisam estar constantemente operacionais, com tolerância a falhas.
- **Desempenho**: aproveita a eficiência da VM Erlang, conhecida por sua baixa latência e alta taxa de transferência.
- **Comunidade ativa**: Uma comunidade crescente e acolhedora, com muitos recursos e bibliotecas.

<img src="https://www.pngkey.com/png/full/935-9356922_880-x-495-4-phoenix-framework-logo.png" align="right" height="77">

A linguagem também tem suporte nativo a hot code swapping (atualização de código sem desligar o sistema) e uma comunidade ativa que fornece ferramentas robustas como o framework web **Phoenix**, que oferece desempenho comparável ao de aplicações escritas em linguagens compiladas. Em resumo, Elixir é uma linguagem moderna construída para resolver problemas complexos de concorrência e distribuição de forma eficiente, segura e elegante.

## [Elixir] Hello, World!
Depois de instalar o Elixir, podemos usar o IEx (Interactive Elixir), um REPL (Read-Eval-Print Loop) interativo que permite executar comandos do Elixir em tempo real.

Para iniciar o IEx, abra seu terminal e digite:

```sh
iex
```

Você verá um prompt interativo onde poderá começar a digitar comandos Elixir.

Agora, vamos criar um programa simples que imprima `"Hello, World!"` no console. Crie um arquivo nomeado com o seguinte conteúdo: `hello.exs`

[![hello.exs](https://img.shields.io/badge/-hello.exs-purple?style=social&logo=Elixir&logoColor=purple)](#)

```elixir
IO.puts("Hello, World!")
```

Para executar o programa, use o comando:

```sh
elixir hello.exs
```

## [Elixir] Comentários

# ⚗️ [Elixir] Tipos de dados

# ⚗️ [Elixir] Operadores e expressões

# ⚗️ [Elixir] Listas e Mapas

# ⚗️ [Elixir] Estruturas de programação

# ⚗️ [Elixir] Módulos

# ⚗️ [Elixir] Funções

# ⚗️ [Elixir] Recursão

# 📦 [Elixir] Hex
<a href="https://hex.pm/"><img src="https://github.com/user-attachments/assets/6e2b2e58-a17c-437a-8f55-8eb75621aeb6" align="right" height="77"></a>

**Hex** é o gerenciador de pacotes oficial do ecossistema Elixir e Erlang, responsável por permitir que desenvolvedores compartilhem, publiquem e reutilizem bibliotecas de forma prática, segura e integrada ao fluxo de desenvolvimento. Ele funciona de maneira semelhante a ferramentas como o npm no JavaScript, o pip no Python ou o Cargo no Rust, sendo utilizado principalmente em conjunto com a ferramenta Mix, que é quem interage diretamente com o Hex durante a instalação e gerenciamento das dependências de um projeto.

Quando um desenvolvedor cria uma biblioteca Elixir que pode ser útil para outras aplicações, ele pode empacotá-la e publicá-la no Hex, permitindo que qualquer pessoa a adicione ao seu próprio projeto com apenas algumas linhas no arquivo `mix.exs`. O Mix então usa o Hex para buscar essa dependência, baixá-la do repositório oficial, compilá-la e deixá-la disponível no ambiente do projeto. Essa integração torna o processo extremamente fluido, removendo a necessidade de downloads manuais ou configurações complicadas de caminhos e versões.

Além de permitir o uso de bibliotecas públicas, o Hex também oferece suporte para repositórios privados, autenticação, gerenciamento de versões e publicação de pacotes com metadados bem definidos, como documentação, dependências transitivas e compatibilidade de versões. Isso o torna uma ferramenta útil tanto para projetos abertos quanto para soluções corporativas internas.

Outro destaque do Hex é seu foco em segurança e confiabilidade. Ele verifica a integridade dos pacotes com checksums, garante que as versões não sejam sobrescritas após publicadas e promove boas práticas de versionamento semântico. Tudo isso contribui para a estabilidade do ecossistema, tornando o uso de bibliotecas de terceiros mais confiável.

Em resumo, o Hex é um componente essencial do ecossistema Elixir, viabilizando a colaboração entre desenvolvedores e acelerando o desenvolvimento de aplicações robustas e bem estruturadas. Sua combinação com o Mix forma uma dupla poderosa, que simplifica a instalação de dependências, organiza o ciclo de vida dos pacotes e fortalece a base de projetos em Elixir com eficiência e praticidade.


# ⚗️ [Elixir] Mix
<a href="https://elixirschool.com/pt/lessons/basics/mix/"><img src="https://github.com/user-attachments/assets/c6fbe669-7088-47d7-b700-ae5c4d8e19c5" align="right" height="77"></a>

**Mix** é a ferramenta oficial de construção (`build`) e gerenciamento de projetos no ecossistema Elixir. Ela oferece uma série de funcionalidades integradas que tornam o desenvolvimento muito mais produtivo, desde a criação de novos projetos até a compilação, gerenciamento de dependências, execução de testes e geração de documentação. Mix é ao Elixir o que ferramentas como Maven são para o Java ou o que Cargo é para o Rust, porém com uma sintaxe mais simples, alinhada à filosofia funcional e enxuta do Elixir.

Quando você cria um novo projeto com Elixir, é o Mix quem estrutura automaticamente os diretórios, arquivos de configuração, e define o ambiente inicial da aplicação. Ele gera um arquivo chamado `mix.exs`, que atua como o coração da aplicação: ali você define o nome do projeto, versão, dependências externas e configurações específicas de compilação. O código-fonte geralmente vai para a pasta `lib`, enquanto os testes ficam em `test`, seguindo convenções já pré-configuradas que ajudam a manter a organização e a consistência no projeto.

Além disso, Mix permite executar tarefas automáticas com muita facilidade. Comandos como `mix compile` compilam o projeto, `mix test` executa a suíte de testes e `mix run` executa código personalizado. Mix também é extensível: você pode criar suas próprias tasks e usá-las como parte de workflows mais complexos, o que o torna muito poderoso em projetos maiores ou com necessidades específicas.

Outro papel fundamental do Mix é integrar com o **Hex**, o gerenciador de pacotes do Elixir. Quando você adiciona uma dependência no `mix.exs` e executa `mix deps.get`, o Mix se encarrega de baixar, compilar e organizar todas as bibliotecas externas necessárias para o seu projeto funcionar. Isso torna a gestão de bibliotecas extremamente simples e transparente, sem necessidade de configuração manual.

Em suma, Mix é mais do que uma simples ferramenta de build: ele é o motor que sustenta a produtividade e o fluxo de desenvolvimento no Elixir. Ele facilita a padronização, automatiza tarefas do dia a dia e traz consigo o espírito funcional, claro e direto que é característico da linguagem Elixir. Dominar o uso do Mix é um passo essencial para qualquer desenvolvedor que queira trabalhar com Elixir de maneira séria e profissional.

Gere um novo projeto Elixir com um único comando:

```sh
mix new friends
```

# 🧪 [Elixir] DDD, BDD e TDD
**DDD (Domain-Driven Design)**, **BDD (Behavior-Driven Development)** e **TDD (Test-Driven Development)** podem ser aplicados em Elixir, embora com algumas adaptações ao estilo funcional e às convenções da linguagem. Abaixo explico como cada um desses paradigmas se encaixa no ecossistema Elixir:

Elixir permite a aplicação de DDD, especialmente quando você utiliza **Phoenix** (framework web popular da linguagem), que oferece suporte a **contextos** — um conceito diretamente inspirado em DDD.

* **Contextos** em Phoenix são usados para **organizar o domínio em módulos bem definidos**, promovendo separação de responsabilidades.
* Em vez de classes ou objetos, você organiza **funções puras e structs** dentro de módulos.
* Você pode modelar **Entidades** (com `defstruct`), **Value Objects**, **Serviços de Domínio** (como funções puras que representam comportamentos) e até **Repositórios** (módulos responsáveis por interagir com o banco, normalmente via `Ecto.Repo`).

Exemplo:

```elixir
defmodule MyApp.Accounts.User do
  defstruct [:id, :name, :email]
end

defmodule MyApp.Accounts do
  alias MyApp.Accounts.User

  def get_user!(id), do: # busca no banco com Ecto
  def register_user(attrs), do: # lógica de criação
end
```

TDD (Test-Driven Development) em Elixir tem suporte excelente a testes, com o framework `ExUnit` incluso por padrão.

* A abordagem TDD (escreva o teste antes da implementação) funciona muito bem porque **Elixir incentiva funções puras e modulares**, o que facilita a testabilidade.
* O uso de `mix test` é super rápido, e ferramentas como `ExCoveralls` ajudam a medir cobertura de testes.

Exemplo de teste TDD com ExUnit:

```elixir
defmodule MyApp.MathTest do
  use ExUnit.Case

  test "soma dois números" do
    assert MyApp.Math.add(1, 2) == 3
  end
end
```

BDD (Behavior-Driven Development) em Elixir, embora Elixir venha com `ExUnit` como padrão, você pode usar ferramentas como **`espec`** ou **`white-bread`** para testes no estilo BDD.

* Com o `espec`, você pode escrever testes com uma sintaxe parecida com o **RSpec do Ruby**.
* Com o `white-bread`, é possível escrever **cenários no estilo Gherkin**, semelhante ao Cucumber, para descrever comportamentos em linguagem natural.

Exemplo com `espec`:

```elixir
describe "User registration" do
  it "creates a user with valid data" do
    result = Accounts.register_user(%{email: "test@example.com", password: "123456"})
    expect(result).to be_ok
  end
end
```

Resumo comparativo no contexto de Elixir:

| Conceito | Como se aplica em Elixir                                                                   |
| -------- | ------------------------------------------------------------------------------------------ |
| **DDD**  | Utilização de contextos, structs e funções puras para modelar domínios.                    |
| **TDD**  | `ExUnit` nativo e altamente integrado com ferramentas como `mix test`.                     |
| **BDD**  | Pode ser usado com bibliotecas como `espec`, `white-bread` ou mesmo com `ExUnit` adaptado. |
