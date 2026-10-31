# Fanfic Archive Theme - Tema de Arquivo de Fanfics

**[English](#english) · [Português](#português)**

---

<a id="english"></a>
# English

A minimalist Tumblr theme with light and dark modes, a three-column layout and an AO3-style "Sort and filter" panel.

## Features

- **Header** with the blog title and a short description.
- **Left sidebar** with a photo and links.
- **Centered posts** (all post types supported).
- **Right panel "Sort and filter"**, inspired by archiveofourown.org: include/exclude tags and post types, search within results, sort by date or notes.
- **Light and dark mode** with a toggle button (top right). It follows the visitor's system setting by default and remembers their choice.
- **Responsive**: on small screens the sidebar and filter stack above the posts, and the filter becomes collapsible.

## Installation

1. Log in to Tumblr and open your blog's **Customize** (Edit appearance) page.
2. Click **Edit theme**, then **Edit HTML**.
3. Delete everything in the editor and paste the full contents of `tema-tumblr-minimal.html`.
4. Click **Update preview**, then **Save**.

## Theme options

After installing, open **Customize → Edit theme**. These options appear in the left panel:

| Option | What it does |
|---|---|
| **Light Background / Light Text / Light Accent** | Colors used in light mode. |
| **Dark Background / Dark Text / Dark Accent** | Colors used in dark mode. |
| **Sidebar Photo** | Photo shown in the left sidebar. If empty, your blog avatar is used. |
| **Filter Tags** | Which tags can be picked in the filter (see below). |
| **Link 1–4 Label / URL** | Extra links in the sidebar. A link only appears when its *Label* is filled in. |

> ⚠️ The option names are in English. If you used an earlier version of this theme with other names, the old settings are not carried over: fill them in again.

### Sidebar links

The sidebar always shows **Home**, **Archive** and **RSS**. It also shows:

- Your **custom pages** (create them in Customize → *Add a page*).
- An **Ask** link, if you enabled asks in your blog settings.
- The **Link 1–4** entries you filled in.

### Choosing which tags appear in the filter

Use the **Filter Tags** option. Type the tags separated by commas:

```
art, writing, personal, photography
```

- Only these tags appear in the filter list, in the order you typed them.
- Case doesn't matter and the `#` is optional (`Art`, `art` and `#art` are the same).
- A tag only shows up on pages where at least one post uses it.
- Leave the field **empty** to list every tag found in the posts of the current page.
- When a list is set, the "Other tags to include/exclude" boxes also accept only the tags from your list.

## Using the filter

Open the **Sort and filter** panel on the right.

| Control | How it works |
|---|---|
| **Sort by** | Date (newest), Date (oldest) or Notes (most notes). |
| **Post type** | Include/Exclude by type: Text, Photo, Quote, Link, Chat, Audio, Video, Answer. Only appears if the page has more than one type. |
| **Tags** | Tick **Include** to keep only posts with that tag, or **Exclude** to hide posts that have it. Numbers show how many posts on the page use each tag. |
| **Other tags to include / exclude** | Type a tag and press Enter (or comma) to add it as a chip. Click ✕ to remove it. Shown only when there are more than 10 tags. |
| **Search within results** | Matches words in the post text and tags. |
| **Sort and filter** | Applies your choices. |
| **Clear filters** | Resets everything. |

**Rules:**

- Several **included tags** → a post must have **all** of them.
- Several **included post types** → a post can match **any** of them.
- **Excluded** tags or types always remove the post.
- A tag can't be both included and excluded: ticking one unticks the other.

### Important limitation

The filter works on the **posts loaded on the current page** (Tumblr paginates the blog). To browse the whole blog by one tag, include only that tag: a link **"See all posts tagged #tag →"** appears in the results and opens Tumblr's own tag page (`yourblog.tumblr.com/tagged/tag`). Tumblr itself only supports one tag at a time on those pages.

The filter panel only appears on the home, tag and search pages, not on individual post pages.

## Light / dark mode

- Click the round button at the top right of the header to switch.
- The choice is saved in the visitor's browser.
- Change the colors of each mode in **Customize → Edit theme**.

## Custom CSS

The theme uses CSS variables, so you can restyle it from the **Custom CSS** field of the theme editor (or by editing the `<style>` block):

```css
:root { --accent: #e11d48; }                 /* light-mode accent */
html[data-theme="dark"] { --accent: #fb7185; } /* dark-mode accent */
.main { max-width: 700px; }                  /* wider post column */
```

Main variables: `--bg`, `--fg`, `--accent`, `--muted`, `--line`, `--soft`.

## Troubleshooting

| Problem | Solution |
|---|---|
| A tag is missing from the filter | It may not be used by any post on the current page, or it isn't in your **Filter Tags** list. Check the spelling. |
| The filter panel is empty or hidden | Posts without tags have nothing to filter by. Post type filters need at least two different types on the page. |
| The filter doesn't work in the editor preview | Check on the live blog (`yourblog.tumblr.com`). |
| A sidebar link doesn't show | Fill in its **Label** as well as its **URL**. |
| My colors went back to default | The option names changed in this version. Set them again under *Edit theme*. |
| The filter panel is closed on my phone | That's intended on small screens. Tap **Sort and filter** to open it. |

---

<a id="português"></a>
# 🇧🇷 Português

Um tema minimalista para Tumblr com modo claro e escuro, layout de três colunas e um painel "Sort and filter" inspirado no filtro do AO3.

## Recursos

- **Header** com o título do blog e uma descrição curta.
- **Sidebar à esquerda** com foto e links.
- **Posts centralizados** (todos os tipos de post são aceitos).
- **Painel "Sort and filter" à direita**, inspirado no archiveofourown.org: incluir/excluir tags e tipos de post, pesquisar nos resultados e ordenar por data ou notas.
- **Modo claro e escuro** com botão para alternar (canto superior direito). Por padrão segue a configuração do sistema do visitante e lembra a escolha dele.
- **Responsivo**: em telas pequenas, a sidebar e o filtro ficam acima dos posts, e o filtro vira um painel que abre e fecha.

## Instalação

1. Entre no Tumblr e abra **Customize** (Editar aparência) do seu blog.
2. Clique em **Edit theme** (Editar tema) e depois em **Edit HTML** (Editar HTML).
3. Apague tudo o que estiver no editor e cole o conteúdo completo de `tema-tumblr-minimal.html`.
4. Clique em **Update preview** (Atualizar prévia) e depois em **Save** (Salvar).

## Opções do tema

Depois de instalar, abra **Customize → Edit theme**. Estas opções aparecem no painel da esquerda:

| Opção | O que faz |
|---|---|
| **Light Background / Light Text / Light Accent** | Cores do modo claro. |
| **Dark Background / Dark Text / Dark Accent** | Cores do modo escuro. |
| **Sidebar Photo** | Foto exibida na sidebar. Se estiver vazia, usa o avatar do blog. |
| **Filter Tags** | Quais tags podem ser escolhidas no filtro (veja abaixo). |
| **Link 1–4 Label / URL** | Links extras na sidebar. O link só aparece quando o *Label* está preenchido. |

> ⚠️ Os nomes das opções estão em inglês. Se você usou uma versão anterior do tema com outros nomes, as configurações antigas não são aproveitadas: preencha-as de novo.

### Links da sidebar

A sidebar sempre mostra **Home**, **Archive** e **RSS**. Também aparecem:

- Suas **páginas personalizadas** (crie em Customize → *Add a page*).
- O link **Ask**, se você ativou perguntas nas configurações do blog.
- As entradas **Link 1–4** que você preencheu.

### Escolher quais tags aparecem no filtro

Use a opção **Filter Tags**. Digite as tags separadas por vírgula:

```
art, writing, personal, photography
```

- Só essas tags aparecem na lista do filtro, na ordem em que você digitou.
- Maiúsculas e minúsculas não importam, e o `#` é opcional (`Art`, `art` e `#art` são a mesma tag).
- Uma tag só aparece nas páginas em que pelo menos um post a usa.
- Deixe o campo **vazio** para listar todas as tags encontradas nos posts da página atual.
- Quando há uma lista definida, as caixas "Other tags to include/exclude" também aceitam apenas as tags da sua lista.

## Usando o filtro

Abra o painel **Sort and filter** à direita.

| Controle | Como funciona |
|---|---|
| **Sort by** | Date (newest) = mais recentes, Date (oldest) = mais antigos ou Notes (most notes) = mais notas. |
| **Post type** | Incluir/Excluir por tipo: Text, Photo, Quote, Link, Chat, Audio, Video, Answer. Só aparece se a página tiver mais de um tipo. |
| **Tags** | Marque **Include** para ver só os posts com a tag, ou **Exclude** para esconder os posts que a têm. Os números mostram quantos posts da página usam cada tag. |
| **Other tags to include / exclude** | Digite uma tag e aperte Enter (ou vírgula) para adicioná-la como chip. Clique no ✕ para remover. Só aparece quando há mais de 10 tags. |
| **Search within results** | Procura palavras no texto dos posts e nas tags. |
| **Sort and filter** | Aplica as suas escolhas. |
| **Clear filters** | Limpa tudo. |

**Regras:**

- Várias **tags incluídas** → o post precisa ter **todas** elas.
- Vários **tipos de post incluídos** → o post pode ser de **qualquer um** deles.
- Tags ou tipos **excluídos** sempre removem o post.
- Uma tag não pode estar em Include e Exclude ao mesmo tempo: marcar uma desmarca a outra.

### Limitação importante

O filtro funciona nos **posts carregados na página atual** (o Tumblr divide o blog em páginas). Para navegar pelo blog inteiro usando uma tag, inclua só essa tag: aparece nos resultados o link **"See all posts tagged #tag →"**, que abre a página de tag do próprio Tumblr (`seublog.tumblr.com/tagged/tag`). O Tumblr aceita apenas uma tag por vez nessas páginas.

O painel de filtro aparece só na página inicial, nas páginas de tag e nas buscas, e não aparece na página de um post individual.

## Modo claro / escuro

- Clique no botão redondo no canto superior direito do header para alternar.
- A escolha fica salva no navegador do visitante.
- Mude as cores de cada modo em **Customize → Edit theme**.

## CSS personalizado

O tema usa variáveis CSS, então você pode mudar o visual pelo campo **Custom CSS** do editor de tema (ou editando o bloco `<style>`):

```css
:root { --accent: #e11d48; }                 /* destaque no modo claro */
html[data-theme="dark"] { --accent: #fb7185; } /* destaque no modo escuro */
.main { max-width: 700px; }                  /* coluna de posts mais larga */
```

Variáveis principais: `--bg`, `--fg`, `--accent`, `--muted`, `--line`, `--soft`.

## Solução de problemas

| Problema | Solução |
|---|---|
| Uma tag não aparece no filtro | Talvez nenhum post da página atual a use, ou ela não está na lista de **Filter Tags**. Confira a grafia. |
| O painel de filtro está vazio ou escondido | Posts sem tags não têm o que filtrar. O filtro de tipo precisa de pelo menos dois tipos diferentes na página. |
| O filtro não funciona na prévia do editor | Teste no blog publicado (`seublog.tumblr.com`). |
| Um link da sidebar não aparece | Preencha o **Label** além da **URL**. |
| Minhas cores voltaram ao padrão | Os nomes das opções mudaram nesta versão. Configure-as de novo em *Edit theme*. |
| O painel de filtro está fechado no celular | É proposital em telas pequenas. Toque em **Sort and filter** para abrir. |
