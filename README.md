# ✝ O Terço — Aplicativo de Oração Católica

Guia completo para rezar o Santo Rosário de Nossa Senhora, com áudio, modo offline e lembretes diários.

## Funcionalidades

- ✝ Guia passo a passo por todas as orações do Terço completo
- 🌸 Todos os 4 mistérios (Gozosos, Dolorosos, Gloriosos, Luminosos)
- 📅 Sugestão automática dos mistérios do dia da semana
- 🔊 Narração em voz alta (Web Speech API — voz em português)
- ⚡ Velocidade de leitura ajustável (0.7x, 0.85x, 1.0x, 1.2x)
- 📴 Modo offline completo (PWA com Service Worker)
- 🔔 Lembretes diários com horário configurável
- 📖 Histórico dos últimos 10 terços rezados
- 📱 Instalável no celular como app nativo

---

## Como Instalar

### Opção 1: Hospedar num servidor (recomendado)

Envie os arquivos para qualquer hospedagem gratuita:

- **Netlify** (mais fácil): arraste a pasta em netlify.com/drop
- **GitHub Pages**: suba no GitHub e ative Pages
- **Vercel**: `npx vercel` na pasta

### Opção 2: Abrir localmente

```bash
# Com Python (já instalado no Mac/Linux):
cd terco-app
python3 -m http.server 8080
# Abrir: http://localhost:8080

# Com Node.js:
npx serve .
```

> ⚠️ Não abra o index.html direto pelo File Explorer — o Service Worker só funciona com servidor HTTP.

---

## Instalar como app no celular

1. Abra o site no **Chrome (Android)** ou **Safari (iPhone)**
2. No Android: toque no menu (⋮) → "Adicionar à tela inicial"
3. No iPhone: toque em Compartilhar (□↑) → "Adicionar à Tela de Início"
4. O app aparecerá como ícone na tela inicial

---

## Ícones

Adicione imagens na pasta `icons/`:
- `icon-192.png` — 192×192 pixels
- `icon-512.png` — 512×512 pixels

Sugestão: use uma cruz ou imagem de Nossa Senhora em fundo dourado.

---

## Estrutura dos arquivos

```
terco-app/
├── index.html      # Aplicativo principal
├── manifest.json   # Configuração do PWA
├── sw.js           # Service Worker (offline)
├── icons/
│   ├── icon-192.png
│   └── icon-512.png
└── README.md
```

---

*Que Nossa Senhora abençoe suas orações. 🌹*
