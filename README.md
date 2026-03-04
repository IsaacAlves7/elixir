<a href=""><img src="https://github.com/user-attachments/assets/7a38b221-ab20-4f6d-b409-b52c37104889"></a>

Sou um especialista em desenvolvimento de software com foco no ecossistema Elixir, aproveitando sua concorrência leve, tolerância a falhas e imutabilidade para criar aplicações escaláveis, resilientes e altamente disponíveis. Domino boas práticas como SOLID, DRY, KISS, TDA e SoC, com aplicação de design patterns funcionais e arquiteturas como Clean Architecture e Domain-Driven Design, assegurando legibilidade, manutenibilidade e escalabilidade do código.

No front-end, atuo em projetos com SPAs (React, Angular, Vue), SSR (Next.js) e design responsivo com HTML/CSS, Flexbox e CSS Grid, baseados em protótipos do Figma (UI/UX).

No back-end, desenvolvo APIs e sistemas distribuídos com Elixir e Phoenix — tanto com REST quanto GraphQL via absinthe — explorando ao máximo o modelo de concorrência baseado em atores do Erlang/OTP. Integro sistemas com canais em tempo real (Phoenix Channels e LiveView), orquestrando fluxos de eventos com GenServers, Tasks, Supervisors e outras abstrações do OTP para garantir robustez e disponibilidade.

Tenho domínio de Git e pipelines CI/CD (GitLab CI, GitHub Actions), utilizo mix para automação de build/testes/lint (com credo, dialyxir, excoveralls), além de testes com ExUnit, Mox e testes de aceitação com Wallaby ou Hound. Faço monitoramento de métricas e telemetria com ferramentas como Prometheus, Grafana e Telemetry.Metrics, além de logging estruturado com Logger e rastreamento de falhas via Sentry.

Em arquiteturas de microsserviços e sistemas event-driven, utilizo mensageria com Kafka, RabbitMQ, ou integração com Broadway para pipelines de dados concorrentes e resilientes. Também atuo com persistência em bancos SQL (PostgreSQL via Ecto) e NoSQL, mantendo consistência e performance com schemas versionados e migrações.

Implemento ferramentas de analytics como Google Analytics 4 ou soluções próprias integradas com o front-end, visando mensurar a usabilidade de features e o comportamento do usuário. Tenho experiência com implantação de sistemas Elixir/Phoenix em produção usando releases (mix release), Docker, Fly.io, Heroku, AWS e Kubernetes, com foco em alta disponibilidade e entrega contínua.

# It's a repository of Elixir programming ⚗️
> ⚗️ **Preparação**: Para este conteúdo, o aluno deverá dispor de um computador com acesso à internet, um web browser com suporte a HTML 5 (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari, Opera etc.), um editor de texto ou IDE (VSCode etc.) e o software Elixir, com a versão mais recente, instalado na sua máquina local.

<a href="https://elixir-lang.org/install.html"><img src="https://github.com/user-attachments/assets/2ca6c1e3-557d-42ab-8a84-3ed8a8a2ad29" align="right" height="77"></a>

O **Elixir** é uma linguagem de programação dinâmica e funcional, concorrente e de propósito geral, projetada para criar aplicações escaláveis e de alta disponibilidade. Ela roda sobre a máquina virtual do Erlang (BEAM), herdando sua robustez e desempenho para sistemas distribuídos, tolerantes a falhas e com forte suporte à concorrência. Elixir é uma linguagem projetada para ser produtiva, com uma sintaxe elegante e moderna, enquanto aproveita a robustez e os recursos de simultaneidade da máquina virtual Erlang.

Criada por José Valim, um desenvolvedor brasileiro e um dos principais contribuidores do framework Ruby on Rails, Elixir surgiu com o objetivo de combinar a solidez da plataforma Erlang — que é usada em sistemas de telecomunicação com tempo de atividade crítico — com uma sintaxe moderna e produtiva, inspirada em linguagens como Ruby. Ele foi criado para ser escalável e manter sistemas de alta disponibilidade, tornando-o uma escolha popular para aplicativos da Web, sistemas distribuídos e telecomunicações. Elixir combina o melhor dos dois mundos: a simplicidade do Ruby e o poder do Erlang.

<img src="https://github.com/user-attachments/assets/8985a54f-1b44-4d20-adc1-bd4094024979" align="right" height="77">

Por que usar o Elixir? O foco do Elixir está em aplicações que exigem alta performance e muitos processos simultâneos, como sistemas financeiros, plataformas de mensagens em tempo real, aplicações IoT, e serviços web escaláveis. Seu modelo funcional evita efeitos colaterais e facilita a manutenção do código, enquanto sua estrutura baseada em processos leves permite criar sistemas que lidam com milhões de conexões simultâneas. 

- **Simultaneidade**: O Elixir facilita a escrita de código simultâneo, aproveitando os processos leves do BEAM.
- **Escalabilidade**: Ideal para aplicativos que precisam lidar com um grande número de conexões simultâneas.
- **Alta disponibilidade**: Projetado para sistemas que precisam estar constantemente operacionais, com tolerância a falhas.
- **Desempenho**: aproveita a eficiência da VM Erlang, conhecida por sua baixa latência e alta taxa de transferência.
- **Comunidade ativa**: Uma comunidade crescente e acolhedora, com muitos recursos e bibliotecas.

<img src="https://www.pngkey.com/png/full/935-9356922_880-x-495-4-phoenix-framework-logo.png" align="right" height="77">

A linguagem também tem suporte nativo a hot code swapping (atualização de código sem desligar o sistema) e uma comunidade ativa que fornece ferramentas robustas como o framework web **Phoenix**, que oferece desempenho comparável ao de aplicações escritas em linguagens compiladas. Em resumo, Elixir é uma linguagem moderna construída para resolver problemas complexos de concorrência e distribuição de forma eficiente, segura e elegante.

## [Elixir] Hello, World!
Depois de instalar o Elixir, podemos usar o **IEx (Interactive Elixir)**, um REPL (Read-Eval-Print Loop) interativo que permite executar comandos do Elixir em tempo real.

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
Em Elixir, comentários são simples e diretos. Eles são feitos com o símbolo `#` e servem para adicionar explicações ou observações no código que não são executadas pelo interpretador.

Tudo que vier após o `#` na mesma linha será ignorado pela compilação:

```elixir
# Este é um comentário de linha
IO.puts("Olá, mundo!")  # Este é um comentário ao lado do código
```

Elixir não possui comentários de múltiplas linhas com sintaxe especial, como `/* ... */` em C ou `""" ... """` em Python. Se quiser escrever um comentário longo, deve usar `#` em cada linha:

```elixir
# Esta função calcula o dobro de um número
# e imprime o resultado no terminal
defmodule Exemplo do
  def dobro(n) do
    IO.puts(n * 2)
  end
end
```

Por fim, é comum em projetos Elixir bem escritos usar comentários para explicar lógicas complexas, mas não para descrever cada linha óbvia — isso porque o estilo idiomático da linguagem preza por código limpo e legível por si só.

# ⚗️ [Elixir] Tipos de dados
Na linguagem **Elixir**, os tipos de dados são imutáveis por natureza e fazem parte de um modelo funcional fortemente influenciado por Erlang. Não existe a separação clássica entre “tipos primitivos” e “tipos complexos” como em linguagens imperativas; todos os valores são dados e tudo é tratado de forma uniforme pelo runtime. Elixir é dinamicamente tipada, mas com tipagem forte, o que significa que conversões implícitas não acontecem silenciosamente e erros de tipo aparecem de forma explícita em tempo de execução.

Em conjunto, esses tipos formam um ecossistema coerente, projetado para imutabilidade, concorrência segura e clareza semântica. Entender bem esses tipos é essencial para escrever código idiomático em Elixir e para evitar armadilhas comuns, principalmente para quem vem de linguagens orientadas a objetos ou imperativas.

Os **números** em Elixir são divididos em inteiros e floats. Inteiros podem ter tamanho arbitrário, não havendo risco de overflow como em linguagens de baixo nível. Floats seguem o padrão IEEE 754 de dupla precisão. Operações entre inteiros e floats não fazem coerção automática; se você soma um inteiro com um float, o resultado é float, mas isso é uma regra explícita do operador, não uma conversão implícita escondida.

```elixir

```

Os **átomos** são um dos tipos mais importantes da linguagem. Um átomo é uma constante cujo valor é o próprio nome, como `:ok`, `:error` ou `:user_created`. Eles são amplamente usados para representar estados, chaves de mapas, identificadores simbólicos e resultados de funções. Um detalhe crítico é que átomos não são coletados pelo garbage collector; criar átomos dinamicamente a partir de entrada externa pode causar vazamento de memória no runtime, o que é uma armadilha clássica para iniciantes.

```elixir

```

As **strings** em Elixir são binários UTF-8, ou seja, sequências de bytes que representam texto. Elas são delimitadas por aspas duplas e diferem bastante de listas de caracteres. Uma string é eficiente para texto, mas não para manipulação caractere a caractere, já que caracteres UTF-8 podem ocupar mais de um byte.

```elixir

```

As **listas** são listas encadeadas (linked lists), ideais para processamento recursivo e padrões funcionais. Elas são representadas por colchetes e podem conter elementos de tipos diferentes. Operações como adicionar no início da lista são eficientes, enquanto acesso aleatório ou concatenação no final têm custo linear. Listas de inteiros entre 0 e 255 têm uma interpretação especial no Elixir e podem representar *charlists*, herdadas do Erlang.

```elixir

```

As **tuplas** são estruturas de tamanho fixo, usadas quando se conhece a quantidade de elementos e se deseja acesso rápido por índice. São muito comuns para retornos de funções, especialmente no padrão `{status, result}`, como `{:ok, value}` ou `{:error, reason}`. Diferente das listas, modificar uma tupla implica criar uma nova cópia completa dela.

```elixir

```

Os **mapas** são estruturas chave–valor e representam a principal forma de modelagem de dados em Elixir moderno. Eles substituíram boa parte do uso de *proplists* e *records* do Erlang. Mapas permitem chaves de qualquer tipo, embora átomos e strings sejam os mais comuns. O acesso e atualização são eficientes e existe uma sintaxe especial quando as chaves são átomos conhecidos em tempo de compilação.

```elixir

```

Os **structs** são mapas com uma forma definida. Eles impõem um conjunto fixo de chaves e são usados para representar entidades do domínio de forma mais segura e expressiva. Embora pareçam classes, structs não têm métodos nem herança; são apenas dados estruturados, alinhados com a filosofia funcional da linguagem.

```elixir

```

Os **binários e bitstrings** são tipos fundamentais para lidar com dados brutos, protocolos, arquivos e comunicação de rede. Um binário é uma sequência de bytes, enquanto bitstrings permitem manipulação em nível de bits. Esse tipo é extremamente poderoso e uma das razões pelas quais Elixir e Erlang são tão fortes em sistemas distribuídos e telecomunicações.

```elixir

```

O tipo **booleano** é, na prática, apenas dois átomos especiais: `true` e `false`. Não existe um tipo boolean separado como em outras linguagens. Isso reforça o papel central dos átomos no sistema de tipos.

```elixir

```

O valor **nil** também é um átomo e representa a ausência de valor. Ele é frequentemente usado como retorno padrão de funções ou para indicar campos vazios, mas, diferente de `null` em outras linguagens, seu uso é mais explícito e menos ambíguo.

```elixir

```

# ⚗️ [Elixir] Operadores e expressões

# ⚗️ [Elixir] Estruturas de programação

# ⚗️ [Elixir] Módulos

# ⚗️ [Elixir] Paradigma Funcional
Por fim, existem os **functions** como tipo de primeira classe. Funções podem ser atribuídas a variáveis, passadas como argumento e retornadas por outras funções. Elas carregam seu próprio escopo, o que viabiliza closures e composições sofisticadas, pilares do estilo funcional adotado pelo Elixir.

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

# 🐦‍🔥 [Elixir] Phoenix
<img src="https://www.pngkey.com/png/full/935-9356922_880-x-495-4-phoenix-framework-logo.png" align="right" height="77">

**Phoenix** é um framework web moderno e de alto desempenho escrito em **Elixir**, uma linguagem funcional baseada na máquina virtual do Erlang (BEAM), conhecida por sua concorrência, tolerância a falhas e escalabilidade. Ele foi criado para fornecer uma maneira eficiente e produtiva de construir aplicações web completas, desde APIs RESTful até interfaces interativas em tempo real com WebSockets e LiveView. Em resumo, o Phoenix é uma ferramenta poderosa para desenvolver aplicações web modernas com foco em desempenho, estabilidade e concorrência, aproveitando os benefícios do Elixir e da plataforma Erlang. É ideal para quem busca criar aplicações robustas, reativas e preparadas para escalar sem complexidade.

Diferente de frameworks tradicionais baseados em linguagens imperativas, como Ruby on Rails ou Django, o Phoenix aproveita os princípios funcionais do Elixir para oferecer um modelo de desenvolvimento imutável, concorrente e altamente confiável. Isso significa que ele é especialmente indicado para aplicações que precisam lidar com **grande volume de conexões simultâneas**, como chats, dashboards ao vivo, notificações em tempo real, jogos multiplayer e sistemas distribuídos.

O Phoenix oferece uma estrutura organizada em camadas, com roteador, controladores, views, templates e canais para comunicação em tempo real. Ele também integra o **Ecto**, a biblioteca oficial de acesso a banco de dados no Elixir, que permite mapear, consultar e migrar dados de forma clara e segura. Além disso, com a tecnologia **LiveView**, o Phoenix permite criar aplicações web interativas e dinâmicas sem usar JavaScript no lado do cliente, mantendo toda a lógica no servidor e atualizando a interface via WebSockets de forma eficiente.

A arquitetura do Phoenix é pensada para escalar com segurança e simplicidade. Ele suporta concorrência nativa, hot reload no desenvolvimento, isolamento de processos, distribuição nativa e comunicação entre nós distribuídos. Tudo isso herdado do poder da BEAM, a máquina virtual do Erlang que vem sendo usada há décadas em sistemas que exigem alta disponibilidade, como telecomunicações e bancos.

Para iniciar uma aplicação com Phoenix, o principal framework web do Elixir, você precisa ter o Elixir e o Phoenix instalados. Supondo que já tenha o ambiente configurado, você pode criar uma aplicação do zero com alguns comandos simples e entender como ela é estruturada com base em exemplos de código reais.

Primeiro, crie o projeto com:

```bash
mix phx.new hello_phoenix
```

Esse comando vai gerar uma estrutura de diretórios completa com suporte a front-end, back-end, banco de dados e WebSocket. Durante a criação, o Mix perguntará se você deseja instalar as dependências e configurar o banco. Confirme com `Y` (yes) quando solicitado.

Depois de criado, entre na pasta do projeto:

```bash
cd hello_phoenix
```

Em seguida, crie e migre o banco de dados:

```bash
mix ecto.create
```

E então inicie o servidor local com:

```bash
mix phx.server
```

Ao abrir o navegador e acessar `http://localhost:4000`, você verá a página inicial padrão do Phoenix, indicando que a aplicação está rodando corretamente.

Dentro do código, um exemplo de controlador básico seria algo assim:

```elixir
defmodule HelloPhoenixWeb.PageController do
  use HelloPhoenixWeb, :controller

  def index(conn, _params) do
    text(conn, "Bem-vindo ao Phoenix!")
  end
end
```

Esse controlador responde a uma requisição com um simples texto. Para conectá-lo a uma rota, edite o arquivo `lib/hello_phoenix_web/router.ex`:

```elixir
scope "/", HelloPhoenixWeb do
  pipe_through :browser

  get "/", PageController, :index
end
```

Esse trecho define que ao acessar a raiz (`/`), a aplicação chamará a função `index` do `PageController`.

Se quiser criar uma nova página com HTML, pode usar a engine de templates EEx. Crie um arquivo `index.html.heex` dentro de `lib/hello_phoenix_web/templates/page/` com o conteúdo:

```html
<h1>Olá, Phoenix!</h1>
<p>Esta é uma página gerada com template HEEx.</p>
```

E altere o controller para renderizar essa view:

```elixir
def index(conn, _params) do
  render(conn, "index.html")
end
```

Esse fluxo já mostra como montar rotas, controladores e templates em Phoenix. A aplicação Phoenix já vem com suporte a PubSub, WebSockets, LiveView, formulários e banco de dados via Ecto. A partir disso, você pode criar schemas, migrar tabelas, lidar com autenticação e desenvolver APIs REST ou interativas com LiveView.

## [Elixir] Phoenix LiveView
**LiveView** normalmente se refere ao **Phoenix LiveView**, uma tecnologia do ecossistema Elixir. O nome completo mais conhecido é **Phoenix LiveView**, que faz parte do framework web **Phoenix Framework**.

LiveView é uma forma de construir interfaces web interativas **sem escrever JavaScript pesado no frontend**. A lógica da interface roda no servidor (em Elixir), e o navegador recebe apenas as atualizações de estado via WebSocket.

Em vez de: Frontend (React/Vue/etc.) ↔ API REST ↔ Backend

Você tem: Browser ↔ WebSocket ↔ LiveView no servidor

Quando algo muda (clique, formulário, evento), o navegador envia o evento para o servidor. O servidor processa, atualiza o estado e envia apenas o “diff” do HTML de volta. O DOM é atualizado automaticamente.

Isso é possível porque o Elixir roda na BEAM (a mesma VM do Erlang), que é extremamente eficiente para lidar com milhares de conexões simultâneas.

Na prática, LiveView permite:

– Atualizações em tempo real
– Formulários reativos
– Validação instantânea
– Dashboards ao vivo
– Chats
– Sem SPA complexa

Tudo com renderização server-side.

É diferente de frameworks tradicionais porque:

– Não é SPA puro
– Não é apenas SSR estático
– Não depende de grandes bundles JS
– Mantém estado no servidor

Conceitualmente, ele é parecido com:

– Hotwire (Rails)
– Server Components do React
– ASP.NET Blazor Server

Mas com um modelo muito consistente graças ao Elixir. LiveView é uma das partes mais interessantes do ecossistema porque une concorrência massiva com simplicidade de frontend.

## [Elixir] Como o Discord atende 15 milhões de usuários em um único servidor
No início do verão de 2022, a equipe de operações do Discord notou uma atividade incomumente alta em seus painéis. Eles acharam que era um ataque de bot, mas era tráfego legítimo do MidJourney – uma nova comunidade em rápido crescimento para gerar imagens de IA a partir de prompts de texto.

Para usar o MidJourney, você precisa de uma conta no Discord. A maioria dos usuários do MidJourney entra em um servidor principal do Discord. Esse servidor cresceu tão rápido que logo atingiu o antigo limite do Discord de cerca de 1 milhão de usuários por servidor.

<img width="1392" height="825" alt="unnamed" src="https://github.com/user-attachments/assets/5fb4a3db-e158-4b04-bcf6-abd5fb576bc7" />

O Discord corria o risco de perder essa nova comunidade importante se não agisse rápido.

Esta é a história de como a equipe do Discord resolveu criativamente esse desafio. Eles encontraram maneiras de expandir drasticamente o que sua infraestrutura podia suportar – mantendo a comunidade vibrante do MidJourney ativa no Discord.

O **Discord** é um aplicativo de chat popular usado por centenas de milhões de pessoas para se conectar. Originalmente para jogadores, agora todos os tipos de comunidades o usam – desde clubes de caminhada até grupos de estudo e grandes comunidades de jogos.

No Discord, um "servidor" hospeda uma comunidade. Possui canais de chat para discutir tópicos escolhidos pelo dono do servidor.

Internamente, o Discord chama esses servidores de "guildas" – então usaremos esse termo daqui para frente.

![unnamed](https://github.com/user-attachments/assets/5503152a-7c2f-4f09-bcb6-1968ca100d81)

Antes do MidJourney, as maiores guildas tinham cerca de 1 milhão de membros – comunidades enormes de jogos como Roblox e Fortnite.

A equipe de engenharia do Discord achava que 1 milhão de membros era muito próximo do máximo que uma guilda podia suportar. Vamos explorar o porquê – mas primeiro, um pouco de contexto rápido sobre as tecnologias que sustentam o Discord.

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
