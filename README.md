<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/jub0t/Concat@main/assets/concat-mark-dark.png" alt="Concat" width="100" />
</p>

<h1 align="center">Lord Editor de Vídeo (Concat)</h1>
<h3 align="center">O substituto gratuito, de código aberto e multiplataforma para o CapCut.</h3>

<div align="center">

<img src="https://cdn.jsdelivr.net/gh/jub0t/Concat@main/assets/editor.png" alt="Editor Concat" width="100%" />

<p align="center">
  <a href="https://github.com/jub0t/Concat/releases"><img src="https://img.shields.io/github/downloads/jub0t/concat/total?style=flat&logo=github&logoColor=F8F8F8&label=Downloads&labelColor=212123&color=0568FD" alt="Total de Downloads" /></a>
  <a href="https://github.com/jub0t/Concat/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/jub0t/Concat/ci.yml?style=flat&logo=githubactions&logoColor=F8F8F8&label=Build&labelColor=000000" alt="Status da Compilação" /></a>
  <a href="https://github.com/jub0t/Concat/releases"><img src="https://img.shields.io/badge/Vers%C3%A3o-0.2.8-0568FD?style=flat&logo=semver&logoColor=F8F8F8&labelColor=212123" alt="Versão do Concat 0.2.8" /></a>
  <a href="https://discord.gg/DVuPfpXfqP"><img src="https://img.shields.io/badge/Discord-Entrar%20no%20servidor-5865F2?style=flat&logo=discord&logoColor=F8F8F8&labelColor=000000" alt="Entrar no Discord do Concat" /></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/Licen%C3%A7a-AGPL%20v3-0568FD?style=flat&logo=gnu&logoColor=F8F8F8&labelColor=212123" alt="Licença: AGPL-3.0-or-later" /></a>
</p>

<p align="center">
  <a href="https://www.star-history.com/jub0t/concat"><img src="https://api.star-history.com/badge?repo=jub0t/concat&type=rank" alt="Classificação no Star History" height="62" /></a>
  <a href="https://trendshift.io/repositories/191379?utm_source=trendshift-badge&amp;utm_medium=badge&amp;utm_campaign=badge-trendshift-191379" target="_blank" rel="noopener noreferrer"><img src="https://trendshift.io/api/badge/trendshift/repositories/191379/daily?language=Rust" alt="jub0t%2FConcat | Trendshift" width="250" height="55"/></a>
  <a href="https://concatenate.pages.dev/#download"><img src="assets/download_button.svg" alt="Baixar Concat" width="251" /></a>
</p>

**🇧🇷 Português (Brasil)** · [🇬🇧 English](README.md) · [🇩🇪 Deutsch](docs/README.de.md) · [🇪🇸 Español](docs/README.es.md) · [🇫🇷 Français](docs/README.fr.md) · [🇮🇹 Italiano](docs/README.it.md) · [🇳🇱 Nederlands](docs/README.nl.md) · [🇵🇱 Polski](docs/README.pl.md) · [🇷🇺 Русский](docs/README.ru.md) · [🇺🇦 Українська](docs/README.uk.md) · [🇹🇷 Türkçe](docs/README.tr.md) · [🇭🇷 Hrvatski](docs/README.hr.md) · [🇮🇩 Bahasa Indonesia](docs/README.id.md) · [🇻🇳 Tiếng Việt](docs/README.vi.md) · [🇹🇭 ไทย](docs/README.th.md) · [🇯🇵 日本語](docs/README.ja.md) · [🇰🇷 한국어](docs/README.ko.md) · [🇨🇳 简体中文](docs/README.zh-Hans.md) · [🇹🇼 繁體中文](docs/README.zh-TW.md) · [🇸🇦 العربية](docs/README.ar.md) · [🇮🇱 עברית](docs/README.he.md) · [🇮🇷 فارسی](docs/README.fa.md) · [🇮🇳 हिन्दी](docs/README.hi.md) · [🇵🇰 اردو](docs/README.ur.md) · [🇧🇩 বাংলা](docs/README.bn.md)

## Patrocinadores Pagos

<table width="100%">
  <tr>
    <td align="center">
      <a href="https://proxyon.io/?ref=concat"><img src="https://cdn.jsdelivr.net/gh/jub0t/Concat@main/assets/proxyon_sponsor_logo.png" alt="Proxyon" width="80" /></a><br />
      <a href="https://proxyon.io/?ref=concat"><b>Proxyon</b></a><br />
      <sub>Proxies pré-pagos para desenvolvedores<br />Use o código <code>JUB0T</code> para 20% de desconto</sub>
    </td>
  </tr>
</table>

</div>


## Sobre

Concat é um editor de vídeo gratuito e de código aberto e uma alternativa ao CapCut para macOS, Windows, Linux e Android. Ele cobre exatamente o que as pessoas buscam no CapCut: legendas automáticas, texto para fala, remoção de fundo, animação por quadros-chave (keyframes), efeitos e títulos, cortes em múltiplas faixas e exportação em 4K. Sem nenhuma das armadilhas: sem marca d'água, sem necessidade de conta, sem assinatura e sem upload de arquivos.

Tudo roda localmente em um motor Rust nativo com um compositor na GPU. Instale, arraste suas gravações e comece a editar. Os modelos de IA para legendas, vozes e recorte são baixados uma única vez através das Configurações e funcionam totalmente offline depois disso. Seus arquivos de vídeo nunca saem do seu disco rígido.

**Ideal para:** TikTok, Reels e Shorts, vídeos para o YouTube, tutoriais e gravações de tela, clipes de podcasts e memes.

**Também para máquinas:** um servidor MCP integrado para agentes de IA (`concat --mcp`, [configuração](docs/MCP.md)) e uma API JSON-RPC para scripts, permitindo que ferramentas automatizadas também editem vídeos[cite: 8].

## Destaques

- 🚫 **Sem marcas d'água. Sem conta. Sem paywall.** Nunca[cite: 8].
- 🔒 **100% local.** Nada é enviado para a rede. Funciona offline[cite: 8].
- 💬 **Legendas automáticas.** Whisper local. Escolha o tamanho do modelo e obtenha legendas estilizadas na linha do tempo[cite: 8].
- 🗣️ **Texto para fala + clonagem de voz.** Vozes locais gratuitas ou qualquer voz a partir de poucos segundos de gravação de áudio[cite: 8].
- 🧍 **Remoção de fundo.** Pessoas, objetos ou pinte você mesmo a máscara desejada[cite: 8].
- 🎞️ **Quadros-chave (Keyframes).** Posição, escala, rotação, opacidade, volume e parâmetros de efeitos. Editor de curvas integrado[cite: 8].
- ✨ **100 efeitos, filtros e transições.** Renderizados diretamente na GPU, ao vivo na pré-visualização[cite: 8].
- ✂️ **Corte rápido.** Dividir, aparar, ripple, mesclar, congelar quadro e velocidade. Linha do tempo magnética opcional[cite: 8].
- 🎚️ **Múltiplas faixas e múltiplas linhas do tempo.** Vários cortes em um único projeto. Modos de mesclagem, recorte e inversões[cite: 8].
- 📝 **Títulos.** Fontes, traçado, sombra e placas de fundo. Predefinições prontas para começar[cite: 8].
- 🎙️ **Limpeza de voz em um botão.** Redução de ruído, aprimoramento de voz e nivelamento de volume. Além de efeitos como esquilo, robô, telefone e similares[cite: 8].
- 📤 **Exportação.** H.264, HEVC e AV1. Até 4K a 60 FPS com profundidade de cor de 10 bits[cite: 8].
- 🦀 **Motor Rust nativo.** Compositor em GPU, proxies e decodificação por hardware. Navegação fluida em 4K[cite: 8].
- 🤖 **Automatizável.** Servidor MCP integrado para que Claude e outros agentes de IA possam editar com ele ([um comando para configurar](docs/MCP.md)) e API JSON-RPC para scripts[cite: 8]. Compilar a partir do código-fonte adiciona gRPC e ferramenta de linha de comando[cite: 8].
- 🖥️ **macOS, Windows, Linux, Android.** 25 idiomas[cite: 8]. O mesmo aplicativo, os mesmos arquivos de projeto[cite: 8].

## Baixar

Duas formas de acessar[cite: 8]:

1. **[O site oficial](https://concatenate.pages.dev/#download)** entrega a versão correta para sua máquina[cite: 8]. Comece por aqui[cite: 8].
2. **[Lançamentos no GitHub](https://github.com/jub0t/Concat/releases)** reúne todas as compilações para todas as plataformas, com instaladores, pacotes e verificações de integridade (checksums)[cite: 8]. Para quando você quiser escolher manualmente[cite: 8].

Concat está em fase **beta**: funciona, mas ainda possui arestas a aparar[cite: 8]. [Avise-nos](https://github.com/jub0t/Concat/issues) quando encontrar alguma[cite: 8].

**Plataformas**

- ✅ **Windows** · x86_64 (as compilações para ARM estão pausadas, veja [#326](https://github.com/jub0t/Concat/issues/326))[cite: 8]. Instalador setup e arquivo `.msi`[cite: 8]. Se o SmartScreen interromper uma compilação não assinada: **Mais informações** › **Executar assim mesmo**[cite: 8].
- ✅ **macOS** · Intel e Apple Silicon[cite: 8]. Se o macOS recusar abrir uma compilação não assinada: `xattr -dr com.apple.quarantine /Applications/Concat.app`[cite: 8].
- ✅ **Linux** · x86_64 e ARM[cite: 8]. Pacotes `.deb`, `.rpm`, `.AppImage` e pacote para Arch[cite: 8]. Também disponível em Flatpak no **[Flatpark](https://flatpark.org/apps/app.concat.editor/)**, um repositório comunitário Flatpak que empacota o `.deb` x86_64 de cada versão e se atualiza com ele[cite: 8].
- ✅ **Android** · celulares e tablets[cite: 8].
- ✅ **iOS / iPadOS** · iPhone e iPad, via sideload[cite: 8].

✅ Suportado · 🚧 Em desenvolvimento · 🧪 Em fase de testes[cite: 8]

**Requisitos de sistema** e os tamanhos opcionais de modelos estão no [site oficial](https://concatenate.pages.dev/guides/system-requirements)[cite: 8].

**[Política de assinatura de código](CODE_SIGNING.md)**: por que as compilações para Windows ainda não são assinadas e o que o Concat envia pela rede (nada que você não tenha solicitado explicitamente)[cite: 8].

## Compilar a partir do código-fonte

Você precisará do Rust 1.93 ou superior (consulte `rust-version` em `src/Cargo.toml`), das bibliotecas de desenvolvimento do FFmpeg 7+, cmake e um compilador C++[cite: 8].

- **macOS:** `brew install ffmpeg`[cite: 8]
- **Windows:** a partir dos [downloads do FFmpeg para Windows](https://ffmpeg.org/download.html#build-windows), baixe a versão `win64-gpl-shared` do BtbN (a mesma usada no CI), descompacte e aponte `FFMPEG_DIR` para ela[cite: 8]
- **Linux:** use o FFmpeg da sua distribuição se for a versão 7 ou mais recente; caso contrário, use uma compilação `shared` do BtbN configurando `FFMPEG_DIR` como no Windows[cite: 8]

Em seguida:

```sh
cd src
cargo run -p concat          # a janela do editor

Outros comandos úteis:

Bash
cargo build --profile app -p concat   # o binário final de distribuição (fat LTO, stripped)
cargo test                            # executar a suíte de testes
cargo fmt --check && cargo clippy --all-targets -- -D warnings   # verificações do CI
Se você alterar algum texto exibido na interface, execute python3 scripts/locales.py a partir da raiz do repositório para manter o inventário de termos sincronizado[cite: 8]. Todos os detalhes estão em CONTRIBUTING.md[cite: 8].

Como Contribuir
[!IMPORTANT]
A melhor maneira de contribuir é baixar uma versão da página de Lançamentos e usá-la no dia a dia: descubra onde ela falha e aponte onde pode melhorar[cite: 8].

Pronto para programar? O documento CONTRIBUTING.md detalha o ambiente, a estrutura de pastas, as verificações obrigatórias e como as contribuições são licenciadas[cite: 8]. Vai controlar o Concat por script, serviço ou agente? A documentação para desenvolvedores cobre a API do Concat e seus transportes: JSON-RPC e gRPC; o arquivo docs/MCP.md ensina a conectar um agente de IA via MCP[cite: 8]. Esta Discussão foi onde o projeto foi anunciado[cite: 8].

Contribuidores podem solicitar o cargo @Contributor no servidor do Discord: basta pedir[cite: 8].

Histórico de Estrelas
Contribuidores
DMCA
Se você acredita que algo neste repositório, em seus lançamentos ou em um pacote ou modelo distribuído infringe seus direitos autorais, envie um e-mail para jub0trd@gmail.com com a descrição da obra protegida, o link de onde o material infrator aparece aqui, suas informações de contato, uma declaração de boa-fé de que o uso não foi autorizado por você, seu representante ou pela lei, e uma declaração, sob pena de perjúrio, de que a notificação é precisa e de que você é o titular ou está autorizado a agir em nome do titular, com sua assinatura física ou eletrônica; notificações válidas são tratadas prontamente, e qualquer pessoa cujo material tenha sido removido pode enviar uma contra-notificação para o mesmo endereço[cite: 8].