# Instalar a LIO no Claude

> **Versão beta.** Encontrou um problema? Veja [CONTRIBUTING.md](CONTRIBUTING.md).

Instalar a LIO é criar a sua própria cópia dela, dentro da sua conta do Claude. A cópia é sua: os estudos, o grupo e as mensagens ficam nela, e a IA usada é a da sua conta.

Este guia é da **LIO-E (Educacional)**, que aparece na tela como **LIO**. Para a versão de leis, veja o [INSTALAR da LIO-L](https://github.com/JOACYFRANCA/lio-l/blob/main/INSTALAR.md).

| Situação | O que fazer |
|---|---|
| Quero a minha LIO | [Instalar](#1-instalar) |
| Saiu uma versão nova | [Atualizar](#2-atualizar) |
| Alguém me convidou para a LIO dele | [Usar uma LIO compartilhada](#3-usar-uma-lio-compartilhada) |

Testado em 13/10/2026 numa conta Pro e numa conta gratuita do claude.ai: as duas instalaram a LIO e usaram estudo, mediação e aula ao vivo.

---

## 1. Instalar

1. Baixe o arquivo **[lio.html](https://github.com/JOACYFRANCA/lio/blob/main/lio.html)**: na página que abrir, clique no botão de download (seta para baixo, "Download raw file").
2. Abra o Claude **[com o pedido de instalação já escrito](https://claude.ai/new?q=Publique%20o%20arquivo%20anexo%20lio.html%20como%20um%20artefato%20novo%2C%20exatamente%20como%20est%C3%A1%2C%20sem%20alterar%20nada%20no%20c%C3%B3digo.%0ADeclare%20exatamente%20estas%20permiss%C3%B5es%20%28capabilities%29%20na%20publica%C3%A7%C3%A3o%3A%0A%0A%7B%0A%20%22sample%22%3A%20%7B%20%22images%22%3A%20true%20%7D%2C%0A%20%22db%22%3A%20%7B%20%22rules%22%3A%20%5B%0A%20%20%7B%20%22path%22%3A%20%22atividades%22%2C%20%22read%22%3A%20%22view%22%2C%20%22write%22%3A%20%22owner%22%20%7D%2C%0A%20%20%7B%20%22path%22%3A%20%22entregas%22%2C%20%22read%22%3A%20%22owner%22%2C%20%22write%22%3A%20%22owner%22%20%7D%2C%0A%20%20%7B%20%22path%22%3A%20%22entregas%2F%7Bself%7D%22%2C%20%22read%22%3A%20%22interact%22%2C%20%22write%22%3A%20%22interact%22%20%7D%2C%0A%20%20%7B%20%22path%22%3A%20%22aula%22%2C%20%22read%22%3A%20%22view%22%2C%20%22write%22%3A%20%22owner%22%20%7D%2C%0A%20%20%7B%20%22path%22%3A%20%22msg%2Fconfig%22%2C%20%22read%22%3A%20%22view%22%2C%20%22write%22%3A%20%22owner%22%20%7D%2C%0A%20%20%7B%20%22path%22%3A%20%22msg%2Fdados%2Fleitura%22%2C%20%22read%22%3A%20%22view%22%2C%20%22write%22%3A%20%22owner%22%20%7D%2C%0A%20%20%7B%20%22path%22%3A%20%22msg%2Fdados%2Fleitura%2F%7Bself%7D%22%2C%20%22write%22%3A%20%22interact%22%20%7D%2C%0A%20%20%7B%20%22path%22%3A%20%22msg%2Fdados%2Fmembros%22%2C%20%22read%22%3A%20%22view%22%2C%20%22write%22%3A%20%22owner%22%20%7D%2C%0A%20%20%7B%20%22path%22%3A%20%22msg%2Fdados%2Fmembros%2F%7Bself%7D%22%2C%20%22write%22%3A%20%22interact%22%20%7D%0A%20%5D%20%7D%2C%0A%20%22user%22%3A%20%7B%20%22scopes%22%3A%20%5B%22profile%22%5D%20%7D%2C%0A%20%22downloads%22%3A%20%7B%7D%2C%0A%20%22room%22%3A%20%7B%20%22topics%22%3A%20%7B%20%22chamar%22%3A%20%22interact%22%20%7D%20%7D%0A%7D%0A%0ADepois%20de%20publicar%2C%20fixe%20o%20artefato%20na%20barra%20lateral%20e%20me%20diga%20o%20endere%C3%A7o%20dele.)** e anexe o `lio.html` que você baixou. Envie.
3. Se o pedido não aparecer escrito, abra uma conversa nova no Claude, anexe o `lio.html` e cole o pedido abaixo, sem mudar nada:

```
Publique o arquivo anexo lio.html como um artefato novo, exatamente como está, sem alterar nada no código.
Declare exatamente estas permissões (capabilities) na publicação:

{
 "sample": { "images": true },
 "db": { "rules": [
  { "path": "atividades", "read": "view", "write": "owner" },
  { "path": "entregas", "read": "owner", "write": "owner" },
  { "path": "entregas/{self}", "read": "interact", "write": "interact" },
  { "path": "aula", "read": "view", "write": "owner" },
  { "path": "msg/config", "read": "view", "write": "owner" },
  { "path": "msg/dados/leitura", "read": "view", "write": "owner" },
  { "path": "msg/dados/leitura/{self}", "write": "interact" },
  { "path": "msg/dados/membros", "read": "view", "write": "owner" },
  { "path": "msg/dados/membros/{self}", "write": "interact" }
 ] },
 "user": { "scopes": ["profile"] },
 "downloads": {},
 "room": { "topics": { "chamar": "interact" } }
}

Depois de publicar, fixe o artefato na barra lateral e me diga o endereço dele.
```

4. Guarde o endereço que o Claude informar. Ele começa com `https://claude.ai/code/artifact/` e será usado para atualizar.
5. Confira se a LIO ficou **fixada na barra lateral** do Claude. É por lá que você a abre nas próximas vezes, sem precisar voltar a esta conversa. A atualização (seção 2) mantém a LIO fixada.

**Como saber se deu certo:** a LIO abre numa página própria, com "Bom dia" (ou "Boa tarde", "Boa noite") e o seu nome, e pergunta **Como você vai usar a LIO?**

**Se não der certo:**

| O que aconteceu | O que fazer |
|---|---|
| A LIO apareceu só dentro da conversa, sem endereço próprio | O Claude fez um artefato comum de chat, que não guarda dados. Peça de novo, lembrando que é para publicar como artefato com as permissões. |
| O Claude pediu para alterar o arquivo | Não autorize mudanças no código. Copie a mensagem do Claude e registre o problema na aba **[Issues](https://github.com/JOACYFRANCA/lio/issues)** deste repositório. |
| A LIO não ficou fixada na barra lateral | Na mesma conversa, peça: "Fixe na barra lateral o artefato que você acabou de publicar." |
| Não aparece a pergunta "Como você vai usar a LIO?" | Você abriu uma LIO de outra pessoa, não a sua. Veja a seção 3. |

---

## 2. Atualizar

Quando sair uma versão nova da LIO, a sua cópia não muda sozinha.

1. Baixe o **[lio.html](https://github.com/JOACYFRANCA/lio/blob/main/lio.html)** novo, como na instalação.
2. No Claude, anexe o arquivo e cole o pedido abaixo, trocando o endereço pelo da sua LIO:

```
Atualize a minha LIO, no endereço https://claude.ai/code/artifact/COLE-AQUI-O-ENDEREÇO,
com o arquivo anexo lio.html, exatamente como está, sem alterar nada no código.
Publique no mesmo endereço e mantenha as permissões que ela já tem.
```

**Importante:** a atualização precisa ser no **mesmo endereço**. Se o Claude publicar como um artefato novo, os seus estudos e o seu grupo continuam na cópia antiga.

---

## 3. Usar uma LIO compartilhada

Quem foi convidado para a LIO de outra pessoa não precisa instalar nada: basta abrir o link do convite.

- Você entra como **participante**: estuda, recebe as atividades e participa da aula ao vivo.
- A escolha "Como você vai usar a LIO?" e a aba **Mediador** aparecem só para o dono daquela LIO.
- Para mediar o seu próprio grupo, instale a sua LIO (seção 1).
- Funciona também com conta gratuita.

### Para quem media: como convidar

No botão **Compartilhar** da sua LIO, mantenha "Apenas pessoas convidadas", convide cada pessoa pelo e-mail da conta Claude e escolha o nível **Colaborador**. Não use **Editor**: o Editor pode alterar a página e as regras de acesso.

---

LIO · Leitura Inteligente Orientada · co-desenvolvimento humano–IA (ver `DECLARACAO_IA.md`).
