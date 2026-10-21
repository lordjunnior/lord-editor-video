# Contribuindo com o Concat

Obrigado por estar aqui. O Concat é um editor de vídeo que roda inteiramente na máquina do usuário, e ele evolui principalmente através de pessoas usando intensamente e relatando o que quebrou.

## A coisa mais valiosa que você pode fazer

Baixe uma versão da página de [Lançamentos](https://github.com/jub0t/Concat/releases) e edite um vídeo real com ela. Gravações reais encontram o que nenhuma leitura do código-fonte revela. Um bom relatório de erro (o que você fez, o que aconteceu, seu sistema operacional, a mídia utilizada) vale mais do que a maioria dos patches.

Discussões mais longas acontecem na [discussão de contribuição](https://github.com/jub0t/Concat/discussions/3) e no [Discord](https://discord.gg/DVuPfpXfqP)[cite: 15].

## Antes de escrever código

Abra uma issue ou entre no Discord primeiro para qualquer coisa além de uma pequena correção. Grandes áreas do projeto já estão em andamento ou foram intencionalmente adiadas, e não é produtivo revisar um pull request grande que precise ser recusado por motivos que eram invisíveis do lado de fora.

## Configurando o ambiente

Você precisará do Rust (veja `rust-version` em `src/Cargo.toml`), das bibliotecas de desenvolvimento do FFmpeg 7+ (`brew install ffmpeg`; veja `src/README.md` para Windows e Linux), cmake e um compilador C++. Depois:

```sh
cd src && cargo run -p concat
Essa é a janela do editor. Tudo: o motor, a camada de host e a interface Slint, compõe um único espaço de trabalho Cargo em src/.   Estrutura (Layout)CaminhoO que reside alisrc/crates/O motor (core, media, render, effects, export, project), a camada de host (concat-host, concat-speech), a API (concat-api, concat-server), a CLI e concat, a janela do editor Slint   O arquivo src/README.md explica como as crates se encaixam e onde estão os pontos críticos. Leia-o antes de mexer no motor.   VerificaçõesExecute estes comandos antes de abrir um PR:Bashcd src && cargo fmt --check && cargo clippy --all-targets -- -D warnings && cargo test
Se você adicionou ou alterou texto exibido na interface, execute também python3 scripts/locales.py para que o inventário de strings acompanhe; o CI verifica isso. As traduções ficam em um arquivo JSON por idioma; consulte TRANSLATING.md.   Se você adicionou ou alterou um modelo disponível para download, inclua-o em models/manifest.toml bem como na tabela do motor à qual ele pertence, e execute python3 scripts/models.py --check; o CI verifica isso também. Um mantenedor então executa o fluxo de trabalho Mirror models, que busca o modelo, registra seu hash (digest) em ambos os lugares e o publica no espelho do qual o aplicativo faz os downloads.   Escreva o que acontece por meio da fachada log (log::info!, log::warn!, log::error!) em vez da saída padrão ou erro padrão. Cada execução grava <app data>/logs/concat-<data>.log, e uma versão empacotada não possui terminal para nada que vá para outro lugar; CONCAT_LOG=debug aumenta o nível de detalhes. Veja src/crates/concat-host/src/logs.rs.   Novos arquivos de código-fonte precisam de um cabeçalho de licença (veja abaixo). Siga o estilo do código ao seu redor; o motor evita complexidade excessiva de propósito.   Licenciando sua contribuição
O Concat é AGPL-3.0-or-later (LICENSE).   