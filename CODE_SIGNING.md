# Política de assinatura de código

Os lançamentos para Windows ainda não são assinados digitalmente[cite: 14]. O Windows exibe um aviso do SmartScreen antes de executar um programa não assinado (Mais informações › Executar assim mesmo), e onde o Smart App Control estiver ativo, ele recusa a execução por completo[cite: 14]. Assim que o Concat obtiver um certificado de assinatura, todos os lançamentos para Windows serão assinados sob esta política[cite: 14].

## O que será assinado

O programa para Windows (`concat.exe`) e seus instaladores (o instalador setup `.exe` e o pacote `.msi`), compilados a partir deste repositório[cite: 14]. Bibliotecas que o Concat distribui mas não compila a partir de seu próprio código-fonte, como as DLLs do FFmpeg e sherpa-onnx e o ONNX Runtime e runtime do Visual C++ da Microsoft, não são assinadas com este certificado; elas mantêm as assinaturas de seus próprios mantenedores onde aplicável[cite: 14].

## Como um lançamento assinado é feito

- Cada arquivo assinado é compilado pelo GitHub Actions a partir de um commit com tag em https://github.com/jub0t/concat, pelos fluxos de trabalho em `.github/workflows` (`release.yml`, que chama `build-app.yml`)[cite: 14]. Nada compilado na máquina pessoal de um desenvolvedor é assinado[cite: 14].
- Um lançamento só é compilado após os testes passarem no commit marcado com tag, e cada pacote para Windows é executado antes do envio (veja `scripts/ci`)[cite: 14].
- Cada solicitação de assinatura é aprovada manualmente por um aprovador listado abaixo[cite: 14].
- Os fluxos de trabalho e scripts de compilação fazem parte do código-fonte e são revisados como qualquer outra alteração[cite: 14].

## Equipe e funções

| Função | Membros |
| :--- | :--- |
| Committers e revisores | [@jub0t](https://github.com/jub0t) |
| Aprovadores | [@jub0t](https://github.com/jub0t) |

Committers podem alterar o código-fonte sem revisão prévia[cite: 14]. Qualquer alteração de terceiros, como um pull request, é revisada por um revisor antes da mesclagem[cite: 14]. Todos os membros utilizam autenticação de dois fatores no GitHub[cite: 14].

## Política de privacidade

Este programa não transfere nenhuma informação para outros sistemas em rede a menos que expressamente solicitado pelo usuário ou pela pessoa que o instala ou opera[cite: 14]. Concat acessa a rede apenas quando você solicita explicitamente[cite: 14]:

- Configurações › Versão consulta o GitHub para listar os lançamentos ao ser aberto ou ao clicar em Verificar atualizações, e instalar um deles realiza o download direto do GitHub[cite: 14].
- Baixar um modelo (transcrição, fala, recorte) busca os arquivos da fonte selecionada em Downloads em Configurações › Geral, e tenta as outras fontes listadas lá caso aquela falhe[cite: 14].
- A API Remota fica desativada por padrão[cite: 14]. Quando ativada, escuta apenas neste computador (127.0.0.1) a menos que você defina outro endereço, respondendo apenas a clientes que possuam o token correspondente[cite: 14].

Nada é enviado sobre você, seus projetos ou suas mídias, e não existe qualquer tipo de telemetria[cite: 14].