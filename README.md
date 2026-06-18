# Controle de Cheques · RM Estruturas

Sistema de controle de cheques recebidos de clientes e repassados a fornecedores.
Aplicativo de arquivo único (`index.html`), sem servidor e sem dependências de instalação.
Os dados ficam salvos no navegador do próprio computador (`localStorage`).

## Arquivos

- **`index.html`** — o sistema. Já vem com os dados da planilha atual carregados.
- **`dados-iniciais-cheques-rm.json`** — backup dos dados iniciais (mesmas informações), para importar manualmente ou guardar como cópia de segurança.
- **`README.md`** — este arquivo.

## Como subir no GitHub Pages

1. Crie um repositório no GitHub (ex.: `controle-cheques`).
2. Envie o `index.html` para a **raiz** do repositório (pode arrastar pelo site do GitHub: *Add file → Upload files*).
3. No repositório, vá em **Settings → Pages**.
4. Em *Branch*, selecione `main` e a pasta `/ (root)`, e salve.
5. Aguarde alguns instantes; o GitHub mostra a URL pública (algo como `https://SEU-USUARIO.github.io/controle-cheques/`).
6. Abra essa URL — os cheques já aparecem.

## Importante sobre os dados

- Os dados são salvos **neste navegador, neste computador**. Funciona offline.
- O indicador no topo mostra **"Salvo neste PC"** quando está hospedado e persistindo.
- Use o botão **Backup** com frequência para baixar um `.json` de segurança.
  Se você limpar os dados do site, trocar de navegador ou de computador, o conteúdo do `localStorage` é perdido — o backup é a forma de restaurar.

## Como usar

- **Novo lote**: cria um grupo pelo cliente que entregou os cheques (ex.: Refricomp).
- **Lançar cheques**: gerador rápido (quantidade, valor por cheque ou total a dividir, número inicial, 1ª data e periodicidade mensal) + grade editável para ajustar emitente por cheque.
- **Editar em lote**: ajusta banco, valor e data "bom para" de vários cheques de uma vez (útil para preencher os bancos dos cheques importados).
- **Menu (⋮) de cada cheque**: repassar a fornecedor, depositar, marcar compensado/devolvido, estornar, histórico, editar, excluir.
- **CSV**: exporta a lista completa para abrir no Excel.
