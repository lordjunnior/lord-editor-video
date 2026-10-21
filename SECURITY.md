# Política de Segurança

## Versões Suportadas

O Concat está em fase pré-1.0[cite: 8]. As correções são aplicadas apenas na versão secundária atual; versões mais antigas não recebem correções[cite: 8].

| Versão | Suportada |
| :--- | :--- |
| 0.2.x | :white_check_mark: |
| < 0.2 | :x: |

## Relatando uma Vulnerabilidade

Por favor, não abra uma issue pública para relatar problemas de segurança[cite: 8].

Relate de forma privada através do formulário de avisos do GitHub:
https://github.com/jub0t/Concat/security/advisories/new[cite: 8]

Inclua a versão (Configurações › Sobre), a plataforma e os passos para reproduzir o problema[cite: 8]. Uma prova de conceito ajuda; um arquivo de projeto que acione a falha é o que mais ajuda[cite: 8].

O que esperar:

- Uma confirmação de recebimento em até 3 dias[cite: 8].
- Uma atualização pelo menos uma vez por semana enquanto o relatório estiver aberto[cite: 8].
- Se o relatório for aceito: uma correção na próxima versão, um aviso publicado e créditos a você, a menos que prefira não ser mencionado[cite: 8].
- Se for recusado: uma explicação do motivo[cite: 8].

## O que é considerado vulnerabilidade

O Concat roda inteiramente na sua máquina[cite: 8]. Relatórios mais relevantes:

- Um arquivo de projeto, arquivo de mídia, modelo ou pacote de efeitos que cause execução de código, escreva fora da pasta do projeto ou leia arquivos que não foram fornecidos[cite: 8].
- Um modelo baixado ou seu espelho sendo substituído por outro sem que a verificação de hash o detecte[cite: 8].
- O servidor da API (`concat-cli serve`, ou Configurações › Automação) aceitando uma chamada que deveria ter recusado: token ausente ou incorreto, em qualquer endereço, ou um servidor iniciado sem token algum[cite: 8].

Por projeto, e não uma vulnerabilidade: o servidor da API faz tudo o que a pessoa que o iniciou pode fazer naquela máquina, e ele não é criptografado[cite: 8]. Cada conexão apresenta um token, gerado quando nenhum foi definido; vincular a qualquer endereço diferente de 127.0.0.1 deve ficar atrás de algo que forneça segurança de transporte[cite: 8].