# Assets do repositório

Arquivos de imagem usados no README e nas páginas de conteúdo.

| Arquivo | Uso | Status |
|---|---|---|
| `banner.svg` | Banner do topo do README | ✅ pronto (cores oficiais: Magenta `#D60B52` e Black 4 `#525251`) |
| `logo-sem-parar.svg` | Assinatura da marca no rodapé do README | ⬜ **a inserir**, usar o arquivo oficial do Brandbook, versão horizontal, fundo claro |
| `logo-sem-parar-branco.svg` | Versão para fundo escuro (tema dark do GitHub) | ⬜ **a inserir**, versão branca oficial |

## Como inserir a logo oficial

1. Exportar do Brandbook 2.0 as versões **horizontal institucional** (Magenta + Black 4) e **horizontal branca**, em SVG.
2. Salvar nesta pasta com os nomes da tabela acima.
3. No `README.md`, substituir o bloco do rodapé por:

```html
<picture>
  <source media="(prefers-color-scheme: dark)" srcset=".github/assets/logo-sem-parar-branco.svg">
  <img src=".github/assets/logo-sem-parar.svg" alt="Sem Parar" height="40">
</picture>
```

## Regras de uso da marca

- Respeitar a margem de respiro do logo (equivalente à largura da seta do próprio logo). Nenhum elemento pode invadir essa margem.
- Não recolorir, distorcer, rotacionar nem aplicar efeitos.
- Em cobranding, Sem Parar sempre em primeiro lugar.
- O banner deste repositório traz "Sem Parar" em tipografia, nas cores oficiais, e **não** reproduz o logo. Ao inserir o arquivo oficial, substitua o bloco de texto do banner pela logo.
