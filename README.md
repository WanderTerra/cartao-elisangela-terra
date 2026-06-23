# Cartão digital — Elisângela Louveira (Fisioterapeuta · RPG)

Página única, clicável, pronta para o GitHub Pages.

Arquivos:
- `index.html` — o cartão (foto, WhatsApp, Maps, chave Pix com cópia, salvar contato). Autossuficiente, sem dependências externas além das fontes do Google.
- `.nojekyll` — evita que o GitHub Pages processe o site com Jekyll (boa prática para site estático).

---

## Opção A — Pelo site do GitHub (sem terminal)

1. Em github.com, crie um repositório novo, por exemplo `cartao-elisangela-terra` (pode ser **público**; o conteúdo é o mesmo que vai no WhatsApp).
2. Clique em **Add file → Upload files** e arraste o `index.html` e o `.nojekyll`. Commit.
3. Vá em **Settings → Pages**.
4. Em **Build and deployment → Source**, escolha **Deploy from a branch**.
5. Branch: **main** / pasta: **/ (root)**. Salve.
6. Aguarde ~1 minuto. A URL aparece no topo da própria página de Pages.

URL final (repositório de projeto):
```
https://WanderTerra.github.io/cartao-elisangela-terra/
```

## Opção B — Pelo terminal (Git)

```bash
cd deploy
git init
git add .
git commit -m "Cartao digital Elisangela (RPG)"
git branch -M main
git remote add origin https://github.com/WanderTerra/cartao-elisangela-terra.git
git push -u origin main
```

Depois, ative o Pages em **Settings → Pages → Deploy from a branch → main / root**.

---

## Observações

- A cópia da chave Pix com **um toque** só funciona em **HTTPS** — ou seja, depois de publicado no Pages funciona certinho (diferente de abrir o arquivo solto no celular).
- Para atualizar o cartão depois (foto, texto, etc.), basta substituir o `index.html` e commitar de novo.
- Se quiser um endereço mais bonito (domínio próprio), dá para configurar em **Settings → Pages → Custom domain**.
