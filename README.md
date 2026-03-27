<div align="center">

<img src="https://img.shields.io/badge/Lumina-AI-00d4ff?style=for-the-badge&labelColor=0a0c12" alt="Lumina AI" />

# Lumina — Inteligência para seus documentos

**Analise qualquer PDF em segundos com IA. Resumo, insights, chat e muito mais.**

[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-0a0c12?style=flat-square&logo=github&logoColor=white)](https://seuusuario.github.io/lumina)
[![Gemini 2.5 Flash](https://img.shields.io/badge/AI-Gemini%202.5%20Flash-4285F4?style=flat-square&logo=google&logoColor=white)](https://aistudio.google.com)
[![License](https://img.shields.io/badge/License-MIT-00d4ff?style=flat-square)](LICENSE)
[![HTML](https://img.shields.io/badge/Built%20with-HTML%20%2B%20JS-f59e0b?style=flat-square)]()

<br/>

![Lumina Screenshot](https://raw.githubusercontent.com/seuusuario/lumina/main/assets/screenshot.png)

</div>

---

## ✨ O que é o Lumina?

**Lumina** é uma ferramenta web de análise de documentos com IA, 100% no navegador. Faça upload de qualquer PDF e obtenha em segundos:

- 📋 **Resumo em 5 pontos** — os principais tópicos do documento
- 💡 **Explicação simples** — para qualquer pessoa entender
- ⚡ **Insights principais** — o que realmente importa
- 💬 **Chat com o PDF** — pergunte qualquer coisa sobre o conteúdo
- 📖 **Biblioteca integrada** — 70+ clássicos da literatura mundial
- 🔤 **OCR automático** — lê PDFs escaneados via IA
- 🌍 **Tradutor** — 14 idiomas disponíveis
- 📊 **Gerador de planilhas** — extrai dados estruturados
- 🎞️ **Gerador de slides** — cria apresentações automaticamente
- ✏️ **Editor de texto** — edita o conteúdo extraído

---

## 🚀 Demo ao vivo

👉 **[lumina.seuusuario.github.io](https://seuusuario.github.io/lumina)**

---

## 🔧 Como usar

### 1. Rodar localmente

Não precisa de servidor. Basta abrir o arquivo:

```bash
git clone https://github.com/seuusuario/lumina.git
cd lumina
# Abra o index.html no seu navegador
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

### 2. Configurar a chave de API

O Lumina usa a **API Google Gemini** (gratuita):

1. Acesse [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
2. Crie uma chave de API gratuita
3. Cole a chave no campo **"AIzaSy..."** no topo do app
4. Clique em **Salvar** — pronto!

> **Limite gratuito:** 250 req/dia · 10 req/min · sem custo

### 3. Deploy no GitHub Pages

```bash
# 1. Faça fork ou clone deste repositório
# 2. Vá em Settings → Pages
# 3. Source: Deploy from branch → main → / (root)
# 4. Salve — seu app estará em:
#    https://seuusuario.github.io/lumina
```

---

## 🏗️ Arquitetura

```
lumina/
├── index.html          # App completo (single-file)
├── README.md           # Este arquivo
├── LICENSE             # MIT License
├── .gitignore          # Arquivos ignorados
└── assets/
    └── screenshot.png  # Screenshot para o README
```

O Lumina é uma aplicação **single-file** — todo HTML, CSS e JavaScript em um único `index.html`. Isso facilita:
- ✅ Deploy em qualquer lugar (GitHub Pages, Netlify, etc.)
- ✅ Uso offline (abrir localmente sem servidor)
- ✅ Sem dependências externas para instalar
- ✅ Fácil de compartilhar (um arquivo só)

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| **HTML5 + CSS3 + JavaScript** | Base da aplicação |
| **Google Gemini 2.5 Flash** | Análise, chat, OCR, tradução, slides |
| **PDF.js** | Extração e visualização de PDFs |
| **XLSX.js** | Geração de planilhas Excel |
| **Project Gutenberg** | Biblioteca de livros clássicos |
| **GitHub Pages** | Hospedagem gratuita |

---

## 📱 Funcionalidades

### Análise de PDF
- Upload por clique ou drag & drop
- Extração automática de texto
- Análise com IA (resumo, explicação, insights)
- Suporte a PDFs de até 20MB

### Chat Inteligente
- Contexto completo do documento (início + meio + fim)
- Histórico de conversa mantido
- Respostas formatadas com parágrafos e listas
- Cita trechos do documento quando relevante

### Biblioteca
- 70+ livros clássicos organizados por gênero
- Análise direta de qualquer livro
- Visualizador com paginação elegante
- Link para leitura online no Gutenberg

### Ferramentas extras
- **OCR** — extrai texto de PDFs escaneados
- **Tradutor** — 14 idiomas com progresso em tempo real
- **Planilha** — organiza dados do PDF em Excel
- **Slides** — gera apresentação com 5 temas
- **Editor** — edita texto extraído com formatação

---

## ⚙️ Configuração avançada

### Trocar modelo de IA

No `index.html`, procure por `gemini-2.5-flash` e substitua por:

```
gemini-1.5-flash    → Mais rápido, limite maior
gemini-1.5-pro      → Mais preciso, mais lento
gemini-2.5-flash    → Padrão atual (recomendado)
```

### Ajustar tamanho das páginas do leitor

```javascript
const BR_CHARS_PER_PAGE = 3000; // Aumente ou diminua conforme preferir
```

### Ajustar contexto do chat

```javascript
const CHAT_MAX = 90000; // Caracteres enviados ao modelo no chat
```

---

## 🔒 Privacidade

- ✅ Nenhum documento é armazenado em servidores
- ✅ Processamento 100% no seu navegador
- ✅ A chave de API fica salva apenas no seu `localStorage`
- ✅ Sem analytics, sem rastreamento

---

## 🤝 Contribuindo

Contribuições são bem-vindas!

```bash
# 1. Fork o repositório
# 2. Crie uma branch
git checkout -b feature/minha-feature

# 3. Faça suas alterações no index.html
# 4. Commit
git commit -m "feat: adiciona minha feature"

# 5. Push e abra um Pull Request
git push origin feature/minha-feature
```

---

## 📄 Licença

MIT License — veja [LICENSE](LICENSE) para detalhes.

---

<div align="center">

Feito com ☕ e muito CSS dark mode

**[⭐ Star este repositório](https://github.com/seuusuario/lumina)** se o Lumina te ajudou!

</div>
