# AO Store

Loja de aplicativos do Umbrel com o pacote do **AO**.

## Instalar

1. No Umbrel, abra **App Store**.
2. Clique em **Community App Stores** e depois em **Add Community App Store**.
3. Informe a URL deste repositorio.
4. Instale o app **AO**.
5. Abra o app e crie a senha no primeiro acesso.

## O que este repositorio contem

- `umbrel-app-store.yml`: identidade da loja.
- `ao/umbrel-app.yml`: manifesto do app, incluindo as pastas opcionais.
- `ao/docker-compose.yml`: como o app roda no umbrelOS.

A imagem da aplicacao fica em `ghcr.io/jovemdupe/ao`. Ela contem apenas o
programa. Historico, memoria e arquivos ficam no volume de dados do app, no seu
Umbrel.

## Pastas

O app declara dois pontos de montagem opcionais:

- **Arquivos do AO** (`/files`): leitura e escrita.
- **Pasta somente leitura** (`/media`): apenas leitura.

Voce escolhe as pastas em **App > Configuracoes**. Prefira liberar uma pasta
especifica (por exemplo `/Home/AO`) em vez da Home inteira.
