# Política de Privacidade — PreControl (extensão do Chrome)

*Última atualização: 9 de outubro de 2026*

O PreControl é uma extensão independente, desenvolvida por **Gabriel de Jesus
Silva**, que automatiza consultas e lançamentos no portal SISCONDJ. **Não tem vínculo oficial** com os Tribunais de Justiça, com o Banco do Brasil ou com o Conselho Nacional de Justiça.

## Resumo

- A extensão **não coleta, não vende e não envia** dados ao desenvolvedor.
- Não há anúncios, rastreamento, análise de uso (analytics) nem cookies próprios.
- Tudo o que a extensão guarda fica **no navegador do próprio usuário**.
- Os dados só saem do computador para os endereços que **o próprio usuário**
  usa ou configura (o SISCONDJ e, opcionalmente, um sistema de gerenciamento
  indicado por ele).

## Quais dados a extensão acessa

Para funcionar, a extensão lê as telas do SISCONDJ em que o usuário já está
logado. Essas telas contêm dados de processos judiciais e financeiros, como:
número de processo e de conta judicial, saldos, depósitos, alvarás, nomes e
CPF/CNPJ de partes e beneficiários e valores.

A extensão **não lê nem guarda senhas**. O login é feito pelo usuário,
diretamente no portal.

## Onde os dados ficam

| Dado | Onde fica |
|---|---|
| Configurações (endereço do SISCONDJ, filtros, preferências) | Armazenamento local do navegador (`chrome.storage`) |
| Planilha de contas (conta → descrição) escolhida pelo usuário | Armazenamento local do navegador |
| Histórico de depósitos, últimos saldos, provisionamentos, conferências | Armazenamento local do navegador (o histórico com mais de 14 meses é apagado sozinho) |
| Chave de API do sistema de gerenciamento (opcional) | Armazenamento local do navegador; nunca vai dentro do pacote da extensão |
| Relatórios (.xlsx, .txt, PDF) | Pasta `Downloads/PreControl/` do computador do usuário |

Remover a extensão apaga os dados guardados no navegador. Os arquivos em
`Downloads` continuam no computador até o usuário apagá-los.

## Para onde os dados podem ser enviados

1. **SISCONDJ** (`link siscondj configuravel`) — as operações rodam no próprio
   portal, com a sessão do usuário, como se ele estivesse fazendo à mão.
2. **Aplicativo de segurança do Banco do Brasil** (`http://127.0.0.1:65482`,
   no próprio computador) — só quando o usuário pede para assinar alvarás com
   o certificado A3. O documento é entregue ao aplicativo local para
   assinatura; nada sai do computador por esse caminho.
3. **Sistema de gerenciamento (opcional)** — se, e somente se, o usuário
   informar um endereço e uma chave de API em Configurações, a extensão envia
   a esse endereço os relatórios de depósitos, saldos e provisionamentos. O
   Chrome pede permissão para o endereço no momento em que ele é salvo. Esse
   sistema é escolhido e controlado pelo usuário ou pela sua instituição, não
   pelo desenvolvedor.

Nenhum dado é enviado a qualquer outro destino.

## Uso limitado

O uso das informações obtidas pela extensão segue a
[Política de Dados do Usuário da Chrome Web Store](https://developer.chrome.com/docs/webstore/program-policies/user-data-faq),
incluindo os requisitos de **Uso Limitado**: os dados são usados apenas para
oferecer as funções da extensão descritas acima; não são transferidos a
terceiros, não são usados para publicidade nem para avaliar crédito, e não são
lidos por pessoas, exceto pelo próprio usuário.

## LGPD

O tratamento dos dados pessoais exibidos no SISCONDJ é feito pelo usuário, no
exercício das suas funções e sob a responsabilidade da instituição a que
pertence. A extensão é apenas uma ferramenta executada no computador do
usuário; o desenvolvedor não tem acesso a esses dados.

## Contato

Dúvidas sobre esta política: Gabriel de Jesus Silva —
gabrieldjesus588@gmail.com.

Mudanças nesta política serão publicadas nesta mesma página, com a data de
atualização.
