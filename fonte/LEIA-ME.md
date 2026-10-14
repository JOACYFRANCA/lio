# Código-fonte da versão independente da LIO

O código-fonte principal é o `lio.html`, na raiz do repositório (a versão para Claude). Esta pasta guarda o que transforma esse arquivo na versão independente, o `index.html`.

| Arquivo | O que é |
|---|---|
| `local_parts.js` | Camada de capacidades da versão independente: IndexedDB, chave e chamadas à API da Anthropic, downloads, formas de uso (estudar sozinho, mediar, participar) |
| `local_config.js` | Aba Configurações da versão independente |
| `build.py` | Monta a versão independente a partir do `lio.html` (na pasta de cima) e dos dois arquivos acima |

## Gerar a versão independente

```
python3 build.py
```

Gera `lio-local.html`. Renomeie para `index.html` e substitua o da raiz do repositório.

`build.py` troca trechos exatos do código-fonte. Se uma troca não encontrar o trecho esperado, o script
para com um erro que mostra o início do trecho. Isso acontece quando o código-fonte mudou naquele ponto:
ajuste a troca correspondente em `build.py` para o novo texto.

## Publicar a versão do Claude

Veja `INSTALAR.md`, na raiz do repositório.

## Licença

Código sob GNU AGPL 3.0 ou posterior (arquivo `LICENSE`); textos sob CC BY 4.0 (arquivo `LICENSE-TEXTOS`). Copyright © 2026 Joacy Raimundo França.
