# Injeta App

Site do Injeta App, pronto para hospedar no GitHub Pages.

## Como publicar

1. No GitHub, crie um repositório público (por exemplo `injeta-app`).
2. Envie todos os arquivos desta pasta para o repositório (Add file > Upload files).
   O arquivo `.nojekyll` também precisa ir.
3. No repositório: Settings > Pages > em "Branch", escolha `main` e a pasta `/ (root)` > Save.
4. Aguarde alguns minutos. O endereço aparece no topo da página Pages:
   `https://SEU-USUARIO.github.io/injeta-app/`

## Como ligar o domínio próprio (depois de registrar no registro.br)

1. No GitHub: Settings > Pages > Custom domain > digite `www.injetaapp.com.br` > Save.
2. No registro.br, no painel do domínio, em "Configurar endereçamento" (modo avançado de DNS), crie:
   - `www` do tipo CNAME apontando para `SEU-USUARIO.github.io`
   - quatro registros do tipo A no domínio sem `www`:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
3. Quando o GitHub confirmar o domínio, marque "Enforce HTTPS".

## Onde alterar

Tudo fica no arquivo `index.html`:

- Número da central: procure por `central:{fone:`
- Nome e e-mail do responsável: procure por `const RESP=`
- Itens do catálogo: procure por `const CATS=`
- Data da Política de Privacidade e dos Termos: procure por `const VIGENCIA=`
