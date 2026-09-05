# Lígia Rezende · Landing Page

Landing page de página única para a nutricionista **Lígia Rezende**.

Identidade visual (Figma `fTY9xYUm3tYklPk6Xgurio`): tons de creme, marrom e
**rosa antigo** (`#c4788a`), verde do WhatsApp (`#25d366`) nos botões de ação,
títulos em *Playfair Display* e texto em *DM Sans*. Cards com efeito de vidro.

## Arquivos

| Arquivo | Descrição |
|---|---|
| `index.html` | A página completa. HTML + CSS + JS embutidos, sem build. |
| `assets/Ligia1.jpeg` | Foto do herói. |
| `assets/Ligia2.jpeg` | Foto da seção "Sobre mim". |
| `assets/Ligia3.jpeg` | Foto reserva (não usada no momento). |

## Como visualizar localmente

Abra `index.html` no navegador (dois cliques), ou rode um servidor local:

```bash
cd ~/Documents/NutriLigiaRezendeSite
python3 -m http.server 8000
# abra http://localhost:8000
```

## Hospedagem (GitHub Pages)

Site publicado automaticamente pelo GitHub Pages a partir da branch `main`.

- URL atual: https://viniciuscastro999.github.io/Nutri-Ligia-Rezende-Site/
- Domínio próprio (em configuração): `nutriligiarezende.com.br`

**Para publicar uma alteração:** edite o arquivo e faça `git push` na `main`.
O site atualiza sozinho em cerca de 1 minuto.

```bash
git add -A
git commit -m "descrição da mudança"
git push
```

### DNS do domínio (no registro.br)

Registros para o domínio raiz `nutriligiarezende.com.br`:

| Tipo | Nome | Valor |
|---|---|---|
| A | (vazio / @) | `185.199.108.153` |
| A | (vazio / @) | `185.199.109.153` |
| A | (vazio / @) | `185.199.110.153` |
| A | (vazio / @) | `185.199.111.153` |
| CNAME | `www` | `viniciuscastro999.github.io` |

Depois, em **Settings → Pages → Custom domain** no GitHub, informe
`nutriligiarezende.com.br` e marque **Enforce HTTPS**.

## Editar conteúdo

- **Contato:** telefone `5511964051476`, e-mail e Instagram estão no HTML.
  Busque por `api.whatsapp.com`, `mailto:` e `instagram.com`.
- **Cores e fontes:** CSS custom properties no topo do `<style>` em `index.html`
  (`--rose`, `--ink`, `--bg`, `--wa`, `--serif`, `--sans`…).
- **Formulário de agendamento:** monta uma mensagem e abre o WhatsApp; a lógica
  está no `<script>` no fim do arquivo (`bookForm`).
- **Fotos:** substitua os arquivos em `assets/` mantendo os mesmos nomes.
