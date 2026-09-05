# Lígia Rezende — Landing Page

Landing page de página única para a nutricionista **Lígia Rezende**.

Identidade visual (Figma `fTY9xYUm3tYklPk6Xgurio`): tons de creme, marrom e
**rosa antigo** (`#c4788a`), verde do WhatsApp (`#25d366`) nos botões de ação,
títulos em *Playfair Display* e texto em *DM Sans*. Cards com efeito de vidro.

## Arquivos

| Arquivo | Descrição |
|---|---|
| `index.html` | A página completa. HTML + CSS + JS embutidos, sem build. |
| `assets/ligia.jpg` | Foto da Lígia usada no herói (e no "Sobre" como fallback). |
| `assets/ligia-2.jpg` | *(opcional)* segunda foto para a seção "Sobre mim". |

## Como visualizar

Abra `index.html` no navegador (dois cliques), ou rode um servidor local:

```bash
cd ~/Documents/NutriLigiaRezendeSite
python3 -m http.server 8000
# abra http://localhost:8000
```

## Seções

Nav flutuante · Herói ("Cansada de começar toda segunda?") · Sobre mim ·
Como funciona (3 pilares) · Meus serviços (Consulta Avulsa / Acompanhamento) ·
Diferenciais (6 itens) · Depoimentos · Agende sua consulta (com formulário em
etapas que abre o WhatsApp) · Rodapé · Botão flutuante de WhatsApp.

## Editar

- **Contato:** telefone `5511964051476`, e-mail e Instagram estão no HTML —
  buscar por `api.whatsapp.com`, `mailto:` e `instagram.com`.
- **Cores e fontes:** CSS custom properties no topo do `<style>` em `index.html`
  (`--rose`, `--ink`, `--bg`, `--wa`, `--serif`, `--sans`…).
- **Formulário de agendamento:** monta uma mensagem e abre o WhatsApp; a lógica
  está no `<script>` no fim do arquivo (`bookForm`).
- **Fotos:** substitua `assets/ligia.jpg` (herói, retrato ~3:4) e, se quiser uma
  imagem diferente no "Sobre", adicione `assets/ligia-2.jpg`.
