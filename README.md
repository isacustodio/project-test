# Minha Central Financeira — PWA sem senha

Este é um app pessoal **local-first**. Nenhum lançamento é compartilhado publicamente. Os dados ficam no `localStorage` do navegador/celular e **não** sincronizam com o banco online anterior. Exporte backups JSON periodicamente e mantenha-os em local seguro.

## Instalação
Hospede a pasta via HTTPS na raiz ou em uma subpasta estática; depois abra no Chrome Android e escolha **Instalar aplicativo** ou menu ⋮ > Adicionar à tela inicial. O navegador precisa servir `manifest.webmanifest` com `application/manifest+json`, ícones PNG e `sw.js` no escopo da aplicação. Não basta abrir `index.html` por `file://` para instalar como PWA.

## Uso sem servidor
O `index.html` pode ser aberto sem login para testar a interface, mas recursos de service worker e PWA exigem um endereço HTTPS (ou localhost). Backups JSON são o meio de portabilidade entre aparelhos.