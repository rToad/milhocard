# MilhoCard · Getreide Commodities

Gerador de card diário de cotações de milho para compartilhamento no WhatsApp e redes sociais.

## Como usar

Acesse o link do GitHub Pages, lance os preços do dia e clique em **↓ Baixar PNG**.

## Deploy (primeira vez)

1. Crie um repositório no GitHub (ex: `getreide-milhocard`)
2. Faça upload de todos estes arquivos
3. Vá em **Settings → Pages → Source: GitHub Actions**
4. O deploy roda automaticamente a cada push

## Atualizar dados WASDE mensais

Edite os valores em `src/MilhoCard.jsx` — procure por `DEFAULT_SAFRA`:

```js
const DEFAULT_SAFRA = {
  br_2425: 132.0,  // Brasil 25/26
  br_2324: 136.0,  // Brasil 24/25
  mu_2425: 1301.1, // Mundo 25/26
  mu_2324: 1231.4, // Mundo 24/25
};
```

Faça o commit e o site atualiza automaticamente.
