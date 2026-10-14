# Declaração de autoria e de uso de IA

**Projeto:** LIO-E · Leitura Inteligente Orientada (Educacional) — na tela e no logo, LIO
**Modelo de desenvolvimento:** co-desenvolvimento humano–IA

## Resumo

A LIO foi concebida, especificada e validada por **Joacy Raimundo França**. O código de cada versão é gerado por um agente de IA, no ambiente da própria plataforma (Claude, ChatGPT e Gemini), sob a direção do autor.

As versões são construídas e publicadas **uma de cada vez**: primeiro a do Claude, depois a do ChatGPT e, por último, a do Gemini. Esta declaração é atualizada a cada publicação.

O projeto não reivindica programação manual do autor. A autoria está na concepção, no desenho pedagógico, na especificação, nas decisões de cada versão, nos testes e na curadoria do resultado. O autor responde pelo projeto como um todo, inclusive pela segurança e pela exatidão do conteúdo.

## Objetivos do projeto

1. **Ferramenta de estudo:** um método de estudo ativo para textos densos, com a IA que o usuário já tem.
2. **Demonstração:** mostrar que é possível construir ferramentas educacionais em co-desenvolvimento humano–IA, em plataformas diferentes, a partir de uma especificação comum.

Por causa do objetivo 2, cada versão é construída inteiramente no ambiente da própria IA (Claude, ChatGPT, Gemini), e o processo é registrado no mesmo formato nas três, em `REGISTRO_DESENVOLVIMENTO.md`. O objetivo 1 tem prioridade. As comparações descrevem o que cada ambiente permitiu, com data e evidência, sem eleger vencedor.

## Papéis

| Atividade | Autor | Agente de IA |
|---|---|---|
| Ideia, público e objetivos do projeto | Definiu | — |
| Método pedagógico e regras (tentar primeiro, confiança, revisão espaçada, rodadas) | Definiu e aprovou | Propôs fundamentação e alternativas |
| Especificação das funções | Pediu, revisou e aprovou | Redigiu a partir dos pedidos |
| Código (HTML, CSS, JavaScript) | Não escreveu | Escreveu e corrigiu |
| Pedidos (prompts) que o app envia à IA | Definiu o que pedir e os limites | Redigiu e ajustou |
| Testes automáticos | Definiu o que precisava funcionar | Escreveu e executou |
| Testes de uso e aceitação | Executou e decidiu | Apoiou com relatórios |
| Identidade visual e nome | Escolheu (nome e logo) | Aplicou no código |
| Documentação | Revisou e aprovou | Redigiu |
| Decisões de publicação, licença e privacidade | Decidiu | Informou opções e riscos |

## Situação das versões

| Versão | Situação | Publicação no repositório |
|---|---|---|
| Claude | Beta (versão 29 do artefato) | Outubro de 2026 |
| ChatGPT | Planejada: começa depois da versão para Claude | — |
| Gemini | Planejada: começa depois da versão para ChatGPT | — |

## Versões e ambientes

### Versão para Claude

- **Plataforma:** claude.ai (artefatos), da Anthropic
- **Modelos:** família Claude 5
- **Conta usada:** conta pessoal do autor no claude.ai, plano Pro
- **Período:** 9 a 14 de outubro de 2026
- **Versões:** 1 a 29 do artefato
- **Registro do processo:** `REGISTRO_DESENVOLVIMENTO.md` e histórico de versões na Documentação Técnica, seção "Histórico de desenvolvimento"

### Versão para ChatGPT

- **Plataforma:** ChatGPT, da OpenAI
- **Situação:** ainda não iniciada. Modelos, conta, período e registro serão informados aqui quando a versão for publicada.

### Versão para Gemini

- **Plataforma:** Gemini, do Google
- **Situação:** ainda não iniciada. Modelos, conta, período e registro serão informados aqui quando a versão for publicada.

## Como o processo foi registrado

- **Especificação comum:** as três versões partem, cada uma no seu momento, do documento "LIO — Especificação para as versões Claude, ChatGPT e Gemini" (revisão de 13/10/2026). O documento ainda **não é público**: será publicado junto com a segunda versão. Para comprovar que ele já existia nesta data, registra-se aqui a impressão digital (SHA-256) do arquivo `LIO_Especificacao_Claude_ChatGPT_Gemini.docx` guardado pelo autor:
  `01e6dd8d5e0113d1f1233502f4d57be611d61338dfa1abcb7c484dd2ab5fd513`
  Qualquer pessoa poderá conferir, quando o arquivo for publicado, que ele é o mesmo (por exemplo, com o comando `sha256sum`).
- **Registro de cada versão:** cada versão registra, em ordem, o pedido do autor, o resultado entregue pela IA e a decisão tomada.
- **Evidências:** as conversas principais de desenvolvimento ficam guardadas, por link ou exportação, como evidência do processo.
- **Cabeçalho do código:** o arquivo de cada versão traz no início a plataforma, a data, a versão da especificação e a menção ao co-desenvolvimento.

## Uso de IA dentro da LIO

Além de ter sido feita com IA, a LIO usa IA durante o estudo:
- prepara exercícios e perguntas;
- dá retorno sobre as respostas;
- explica trechos difíceis;
- sugere etiquetas.

A IA é sempre chamada por um botão do usuário. Cada pedido envia só o trecho necessário, e toda citação gerada é conferida contra o texto antes de ser usada.

## Uso acadêmico

A LIO é um projeto independente. Se vier a ser objeto ou ferramenta de um trabalho acadêmico, esta declaração serve como registro público e datado do uso de IA no desenvolvimento. O trabalho acadêmico trará, além dela, a declaração própria exigida pela instituição.

## Observação sobre direitos

A autoria aqui declarada é a do projeto: concepção, especificação, desenho pedagógico e curadoria. A situação jurídica de código gerado por IA ainda não está pacificada. Por isso, a origem do código é informada de forma explícita, e o uso do projeto segue as licenças indicadas nos arquivos LICENSE (código: GNU AGPL 3.0 ou posterior) e LICENSE-TEXTOS (textos e documentação: CC BY 4.0).

## Histórico desta declaração

| Data | Mudança |
|---|---|
| 2026-10-13 | Primeira versão, com a publicação da versão para Claude (beta); especificação comum registrada por impressão digital, ainda não publicada |
| 2026-10-14 | Versões 28 e 29; esta LIO passa a ser chamada também de LIO-E (Educacional), primeira da família LIO, e dá origem à LIO-L (leis), publicada em [github.com/JOACYFRANCA/lio-l](https://github.com/JOACYFRANCA/lio-l) |

