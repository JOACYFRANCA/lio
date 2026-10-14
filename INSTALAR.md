# Instalar a LIO no Claude

> **Versão beta.** Encontrou um problema? Veja [CONTRIBUTING.md](CONTRIBUTING.md).

Instalar a LIO é criar a sua própria cópia dela, dentro da sua conta do Claude. A cópia é sua: os estudos, o grupo e as mensagens ficam nela, e a IA usada é a da sua conta.

| Situação | O que fazer |
|---|---|
| Quero a minha LIO | [Instalar](#1-instalar) |
| Saiu uma versão nova | [Atualizar](#2-atualizar) |
| Alguém me convidou para a LIO dele | [Usar uma LIO compartilhada](#3-usar-uma-lio-compartilhada) |

Testado em 13/10/2026 numa conta Pro e numa conta gratuita do claude.ai: as duas instalaram a LIO e usaram estudo, mediação e aula ao vivo.

---

## 1. Instalar

1. Baixe o arquivo `lio.html` deste repositório (abra o arquivo e clique em **Download raw file**).
2. No Claude, abra uma conversa nova e anexe o `lio.html`.
3. Copie e cole o pedido abaixo, sem mudar nada:

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
| O Claude pediu para alterar o arquivo | Não autorize mudanças no código. Copie a mensagem do Claude e registre o problema na aba **Issues** deste repositório. |
| A LIO não ficou fixada na barra lateral | Na mesma conversa, peça: "Fixe na barra lateral o artefato que você acabou de publicar." |
| Não aparece a pergunta "Como você vai usar a LIO?" | Você abriu uma LIO de outra pessoa, não a sua. Veja a seção 3. |

---

## 2. Atualizar

Quando sair uma versão nova da LIO, a sua cópia não muda sozinha.

1. Baixe o `lio.html` novo deste repositório.
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
