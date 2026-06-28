# 💰 Controle Financeiro

Um app de finanças pessoais simples, rápido e que funciona offline. Feito em um único arquivo HTML, sem servidor, sem cadastro e sem mensalidade. Os dados ficam guardados no seu próprio aparelho.

> Acompanhe entradas, gastos à vista e no cartão de crédito, faturas, assinaturas, reservas e orçamentos — tudo em um lugar.

---

## ✨ O que ele faz

- **Entradas e saídas** — registre o que entra e o que sai, por categoria.
- **Cartão de crédito de verdade** — o app entende fechamento e vencimento. Compras feitas depois do fechamento já caem na fatura seguinte, igual ao cartão real. Suporta **parcelamento** (as parcelas aparecem nas faturas dos meses seguintes sozinhas).
- **Pagar fatura** — quando a fatura fecha, você "paga" e o valor sai do saldo no mês do pagamento, como um débito real.
- **Corrigir valor da fatura** — se a fatura veio diferente da soma (juros, IOF, anuidade), você ajusta o total e o app mostra a diferença discriminada.
- **Vários cartões** — cada um com seu fechamento, vencimento e limite de gasto próprios.
- **Limite de gasto por cartão** — defina um teto mensal e veja uma barra colorida (verde / amarelo / vermelho) avisando quanto já usou. Guarda histórico: se mudar o limite, os meses passados mantêm o valor da época.
- **Assinaturas** — cadastre mensalidades (streaming, academia…) uma vez e elas entram na fatura todo mês automaticamente. Dá pra cancelar (mantendo o histórico) e ver quanto cada uma já custou.
- **Entradas recorrentes** — seu salário e outras receitas fixas entram todo mês sozinhos.
- **Reservas** — guarde dinheiro separado do saldo do mês e resgate quando precisar.
- **Orçamento por categoria** — defina limites e veja quando está perto ou passou.
- **Resumo do mês** — quanto entrou, saiu, pra onde foi o dinheiro, e comparação com o mês anterior.
- **Busca** — encontre qualquer lançamento por descrição, categoria, valor ou mês.
- **Backup e restauração** — exporte tudo para um arquivo e importe de volta quando quiser.
- **Funciona offline** — depois de instalado, abre na hora mesmo sem internet.

---

## 🚀 Como usar

### Online (recomendado)

O app está hospedado no GitHub Pages. Basta abrir o link no navegador:

```
https://noctvictor.github.io/financas/```

### Instalar como aplicativo no celular

Depois de abrir o link, dá pra instalar como um app de verdade (ícone na tela inicial, tela cheia, funciona offline):

- **Android (Chrome):** menu `⋮` → **Instalar app** (ou "Adicionar à tela inicial").
- **iPhone (Safari):** botão de compartilhar `􀈂` → **Adicionar à Tela de Início**.

---

## 💾 Sobre os seus dados

**Importante:** os dados ficam salvos **no navegador do aparelho** onde você usa o app — não em uma nuvem. Isso significa:

- ✅ Funciona offline e é rápido.
- ✅ Seus dados são só seus, ninguém mais acessa.
- ⚠️ Os dados ficam **apenas naquele aparelho**. Não sincronizam entre celular e computador.
- ⚠️ Limpar os dados do navegador, ou desinstalar o app, **apaga tudo**.

### Faça backup de vez em quando

Por isso existe o botão **⬇ Backup**: ele baixa um arquivo com todos os seus dados. Guarde esse arquivo em um lugar seguro (Google Drive, e-mail, etc.).

Para restaurar (em um aparelho novo ou se algo der errado), use **⬆ Importar** e selecione o arquivo de backup.

> O app mostra um lembrete de tempos em tempos sugerindo o backup. Vale a pena fazer com regularidade.

---

## 🧠 Como funciona a fatura do cartão

A fatura depende de duas datas que você configura em cada cartão:

- **Fechamento** — o dia em que a fatura fecha.
- **Vencimento** — o dia em que você paga.

A regra:

- Compras **antes** do dia de fechamento → entram na fatura atual.
- Compras **no dia do fechamento ou depois** → vão para a fatura seguinte.

Exemplo: se o fechamento é dia 2, uma compra feita no dia 4 já entra no próximo ciclo (você ganha mais prazo para pagar). É exatamente como funciona no banco.

---

## 🛠️ Detalhes técnicos

- Um único arquivo `index.html` (HTML + CSS + JavaScript, sem dependências externas).
- `sw.js` é o *service worker* que faz o app funcionar offline.
- Os dados são guardados localmente no navegador.
- Sem build, sem framework, sem servidor.

### Arquivos

| Arquivo | Função |
|---|---|
| `index.html` | O app inteiro |
| `sw.js` | Service worker (modo offline) |

---

## 📄 Licença

Projeto pessoal de uso livre. Sinta-se à vontade para adaptar como quiser.
