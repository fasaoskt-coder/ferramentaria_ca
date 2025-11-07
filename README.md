[README.md](https://github.com/user-attachments/files/23413774/README.md)
# Ferramentaria - Vercel Ready

Arquivos preparados para publicação no Vercel (GitHub → Vercel).

## Como usar

1. Extraia os arquivos ou copie para o seu repositório git na branch que o Vercel monitora (ex.: `main`):
   - `index.html` (arquivo principal)
   - `vercel.json` (configuração para redirecionar todas as rotas para index.html)
   - `README.md` (instruções)
   - `.gitignore` (opcional)

2. Commit e push:
```bash
git add index.html vercel.json README.md .gitignore
git commit -m "Deploy: Ferramentaria app (Vercel-ready)"
git push origin main
```

3. No dashboard da Vercel: escolha o projeto ligado ao repositório e aguarde o deploy. Se o projeto foi detectado como framework (Next.js/React), ajuste em Settings → Framework Preset → **Other** e Output Directory para `.`

4. Verifique o deployment logs em caso de erro. Se tudo certo, o site estará disponível no domínio da Vercel.

## Observações
- Garanta que o site seja servido via HTTPS (Vercel já fornece HTTPS por padrão).
- Se preferir hospedar em uma pasta `public/`, mova `index.html` para `public/index.html` e ajuste `vercel.json` ou Output Directory.
