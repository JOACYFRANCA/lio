# LIO-E · Leitura Inteligente Orientada (Educacional)

> Na tela e no logo, aparece como **LIO**.

> **Versão beta:** em teste. Sua opinião ajuda a definir a versão 1.0 — veja [Contribua](#contribua).

Ferramenta de estudo para quem precisa compreender e memorizar textos densos.
Combina leitura ativa por seções, perguntas de compreensão em três níveis, revisão
espaçada, mapas visuais, fichamento e treino de memória de trabalho.

> **Família LIO:** esta é a **LIO-E (Educacional)**, para textos densos de qualquer área. Para estudar **lei seca** (concursos, Direito), use a **[LIO-L · Leitura Inteligente Orientada de Leis](https://github.com/JOACYFRANCA/lio-l)**, que lê a lei artigo por artigo e treina com itens no estilo das bancas.

## Duas formas de usar

| Forma | Arquivo | Como |
|---|---|---|
| **No Claude** (versão de referência) | `lio.html` | Instale na sua conta do Claude: veja [INSTALAR.md](INSTALAR.md). A IA é a da sua conta; grupo, mensagens e aula ao vivo funcionam pelo próprio Claude. |
| **No navegador** (versão independente) | `index.html` | Abra o site: [https://joacyfranca.github.io/lio/](https://joacyfranca.github.io/lio/). Os estudos ficam no navegador de cada pessoa; a IA usa uma chave da API ou o modo copiar e colar. |

## Contas do Claude

- **Onde foi criada:** a versão de referência foi construída na conta principal do autor, no plano Pro.
- **Usar uma LIO compartilhada:** testado com sucesso em duas contas gratuitas, como participante, inclusive a aula ao vivo.
- **Mediar um grupo:** só quem é dono da LIO (quem a instalou na própria conta) vê a escolha "Como você vai usar a LIO?" e a aba Mediador.
- **Instalar uma cópia própria:** testado com sucesso numa conta gratuita em 13/10/2026; a cópia funcionou como na conta Pro, inclusive a mediação e a aula ao vivo.

## Formas de uso

Na primeira abertura, a LIO pergunta como você vai usá-la. A escolha pode ser mudada
depois, no Início.

| Forma | Para quem | O que aparece |
|---|---|---|
| Estudar sozinho | Uso principal. Cada pessoa prepara e estuda o próprio texto. | As cinco abas de estudo. |
| Mediar um grupo | Quem prepara atividades para outras pessoas. Pode ser um professor ou um colega. | As cinco abas e a aba **Mediador**. |
| Participar de um grupo | Quem recebe uma atividade pronta. | As cinco abas, sem IA e sem chave. |

Exemplo: em um grupo de estudo com três colegas, um deles escolhe **Mediar um grupo**,
prepara a atividade e a envia aos outros dois, que participam.

Links diretos:

| Link | Efeito |
|---|---|
| [https://joacyfranca.github.io/lio/#participante](https://joacyfranca.github.io/lio/#participante) | Abre como participante: sem IA e sem chave. |
| [https://joacyfranca.github.io/lio/#mediador](https://joacyfranca.github.io/lio/#mediador) | Abre já no modo de mediação. |

## Fluxo do grupo

1. O mediador cria um estudo, prepara os exercícios e o teste com a IA, revisa tudo na
   aba **Mediador** e clica em **Exportar arquivo**.
2. O participante abre o site, vai em **Estudar** e usa **Importar atividade recebida (.json)**.
3. Ao fim, o participante exporta o relatório; o mediador importa os relatórios na aba
   **Mediador**.

## Privacidade

- Os dados ficam no navegador de cada pessoa. Apagar os dados de navegação apaga os
  estudos: use **Configurações → Exportar backup**.
- Como participante, nenhum texto é enviado a serviços de IA.
- O registro de uso para pesquisa começa desligado e só registra com consentimento.

## Cuidados com o repositório

- Não coloque neste repositório textos protegidos por direitos autorais nem arquivos de
  atividade com esses textos. Distribua as atividades diretamente aos participantes.
- Nunca coloque uma chave de API em nenhum arquivo do repositório.

## Como foi feito

Co-desenvolvimento humano–IA: concebido, especificado e validado pelo autor; código
gerado pelo Claude (Anthropic) sob a direção do autor. Ver `DECLARACAO_IA.md`.

## Documentação

- [Manual de utilização](docs/Manual_de_Utilizacao_LIO.pdf): como estudar, participar e mediar.
- [Documentação técnica](docs/Documentacao_Tecnica_LIO.pdf): como a LIO funciona por dentro.
- [Declaração de IA](DECLARACAO_IA.md) e [Registro de desenvolvimento](REGISTRO_DESENVOLVIMENTO.md): como a LIO foi feita.

## Licença

| O quê | Licença | Arquivo |
|---|---|---|
| Código: `lio.html`, `index.html` e, no pacote do código-fonte, `build.py`, `local_parts.js` e `local_config.js` | **GNU AGPL 3.0 ou posterior** (AGPL-3.0-or-later) | `LICENSE` |
| Textos e documentação: README, INSTALAR, CONTRIBUTING, Declaração de IA, Registro de desenvolvimento, Manual e Documentação Técnica | **Creative Commons Atribuição 4.0** (CC BY 4.0) | `LICENSE-TEXTOS` |

Copyright © 2026 Joacy Raimundo França. Código gerado por IA sob a direção do autor (ver `DECLARACAO_IA.md`).

Em resumo: você pode usar, estudar, copiar e modificar a LIO. Se distribuir uma versão modificada do código, inclusive como serviço on-line, precisa manter os créditos e oferecer o código-fonte dessa versão sob a mesma licença. Ao reutilizar os textos, cite a autoria e indique se fez alterações. Pedimos ainda que versões modificadas deixem claro que não são a LIO oficial.

Os textos que cada pessoa estuda na LIO continuam sendo de seus autores: estas licenças não se aplicam a eles.

## Contribua

- **Dê sua opinião:** [formulário de 5 minutos](https://docs.google.com/forms/d/e/1FAIpQLSfgBYt45TQsZMBL3DV7KHX-LgpnLY-RDb17_6ggDfYdwDai4Q/viewform), sem login.
- **Encontrou um erro ou tem uma ideia?** Abra uma [Issue](https://github.com/JOACYFRANCA/lio/issues/new/choose) com o modelo **Erro** ou **Sugestão**.
- Veja como as contribuições são tratadas em [CONTRIBUTING.md](CONTRIBUTING.md).

