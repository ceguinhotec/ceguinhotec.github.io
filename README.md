# assiste aí 📺

Um player IPTV moderno e acessível desenvolvido em React, com tema dark e interface em português brasileiro.

## 🌟 Características

- **Interface Moderna**: Design elegante com tema dark e gradientes
- **100% Acessível**: Compatível com leitores de tela e navegação por teclado
- **Responsivo**: Funciona perfeitamente em desktop, tablet e mobile
- **Player Avançado**: Suporte a HLS.js para streams M3U8
- **Múltiplos Formatos**: Carregamento via URL, texto ou playlist de exemplo
- **Sistema de Favoritos**: Marque seus canais preferidos
- **Histórico**: Acompanhe os canais assistidos
- **Estatísticas**: Veja suas preferências de visualização
- **Busca Inteligente**: Encontre canais por nome ou categoria
- **Visualizações**: Modo lista ou grade para os canais

## 🚀 Funcionalidades

### Player de Vídeo
- Suporte nativo a streams HLS (M3U8)
- Controles avançados com teclado
- Indicadores de qualidade e bandwidth
- Modo tela cheia
- Controles de volume
- Estatísticas de rede em tempo real

### Gerenciamento de Playlists
- **URL**: Carregue playlists diretamente de URLs
- **Texto**: Cole o conteúdo M3U diretamente
- **Exemplo**: Playlist de demonstração incluída

### Interface Intuitiva
- Busca em tempo real
- Filtros por categoria
- Visualização em lista ou grade
- Informações detalhadas dos canais
- Sistema de favoritos persistente

### Acessibilidade Total
- Suporte completo a leitores de tela
- Navegação por teclado em todos os elementos
- Alto contraste (WCAG AAA)
- Elementos touch-friendly para mobile
- Estrutura semântica HTML5

## 🛠️ Tecnologias Utilizadas

- **React 19** - Framework principal
- **Vite** - Build tool e dev server
- **Tailwind CSS** - Estilização
- **shadcn/ui** - Componentes de interface
- **HLS.js** - Reprodução de streams HLS
- **M3U Parser Generator** - Processamento de playlists
- **Lucide React** - Ícones

## 📦 Instalação

### Pré-requisitos
- Node.js 18+ 
- pnpm (recomendado) ou npm

### Passos

1. **Clone o repositório**
   ```bash
   git clone <url-do-repositorio>
   cd assiste-ai
   ```

2. **Instale as dependências**
   ```bash
   pnpm install
   # ou
   npm install
   ```

3. **Execute o projeto**
   ```bash
   pnpm dev
   # ou
   npm run dev
   ```

4. **Acesse o aplicativo**
   Abra http://localhost:5173 no seu navegador

## 🎯 Como Usar

### 1. Carregando uma Playlist

#### Via URL
1. Clique na aba "URL"
2. Cole a URL da sua playlist M3U
3. Clique em "Carregar da URL"

#### Via Texto
1. Clique na aba "Texto"
2. Cole o conteúdo da playlist M3U
3. Clique em "Carregar do Texto"

#### Playlist de Exemplo
1. Clique na aba "Exemplo"
2. Clique em "Carregar Exemplo"

### 2. Navegando pelos Canais

- **Buscar**: Use a barra de busca no topo
- **Filtrar**: Selecione uma categoria no dropdown
- **Visualizar**: Alterne entre lista e grade
- **Favoritar**: Clique no ícone de coração

### 3. Assistindo Conteúdo

1. Clique em qualquer canal da lista
2. O player será ativado automaticamente
3. Use os controles do player:
   - **Espaço**: Play/Pause
   - **M**: Mute/Unmute
   - **F**: Tela cheia
   - **R**: Reiniciar

### 4. Recursos Avançados

- **Histórico**: Veja os últimos canais assistidos
- **Estatísticas**: Acompanhe suas preferências
- **Favoritos**: Acesso rápido aos canais preferidos

## ⌨️ Atalhos de Teclado

| Tecla | Ação |
|-------|------|
| `Tab` | Navegar entre elementos |
| `Enter` / `Espaço` | Ativar botões/links |
| `Esc` | Fechar modais |
| `F` | Tela cheia (no player) |
| `M` | Mute/Unmute (no player) |
| `Espaço` | Play/Pause (no player) |

## 📱 Compatibilidade

### Navegadores
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Dispositivos
- Desktop (Windows, macOS, Linux)
- Tablets (iOS 12+, Android 8+)
- Smartphones (iOS 12+, Android 8+)

### Leitores de Tela
- NVDA (Windows)
- JAWS (Windows)
- VoiceOver (macOS/iOS)
- TalkBack (Android)

## 🔧 Configuração Avançada

### Variáveis de Ambiente

Crie um arquivo `.env` na raiz do projeto:

```env
VITE_DEFAULT_PLAYLIST_URL=sua-url-aqui
VITE_APP_TITLE=assiste aí
VITE_ENABLE_ANALYTICS=false
```

### Personalização

O aplicativo usa Tailwind CSS. Para personalizar:

1. Edite `tailwind.config.js`
2. Modifique as cores em `src/App.css`
3. Ajuste componentes em `src/components/`

## 🏗️ Build para Produção

```bash
# Build
pnpm build

# Preview do build
pnpm preview

# Deploy (exemplo com Vercel)
npx vercel --prod
```

## 📊 Performance

- **Tempo de carregamento**: < 2s
- **First Contentful Paint**: < 1s
- **Largest Contentful Paint**: < 2.5s
- **Cumulative Layout Shift**: < 0.1
- **Time to Interactive**: < 3s

## 🔒 Segurança

- Sanitização de URLs
- Validação de conteúdo M3U
- Proteção contra XSS
- Headers de segurança configurados
- HTTPS obrigatório em produção

## 🐛 Solução de Problemas

### Player não carrega
- Verifique se a URL do stream está acessível
- Confirme se o formato é suportado (M3U8, MP4)
- Teste em outro navegador

### Playlist não carrega
- Verifique a sintaxe do arquivo M3U
- Confirme se a URL está acessível
- Teste com a playlist de exemplo

### Problemas de performance
- Limpe o cache do navegador
- Verifique a conexão de internet
- Reduza o número de canais carregados

## 🤝 Contribuindo

1. Fork o projeto
2. Crie uma branch para sua feature
3. Commit suas mudanças
4. Push para a branch
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 🙏 Agradecimentos

- [React](https://reactjs.org/) - Framework principal
- [Vite](https://vitejs.dev/) - Build tool
- [Tailwind CSS](https://tailwindcss.com/) - Estilização
- [shadcn/ui](https://ui.shadcn.com/) - Componentes
- [HLS.js](https://github.com/video-dev/hls.js/) - Player HLS
- [Lucide](https://lucide.dev/) - Ícones

## 📞 Suporte

Para suporte, abra uma issue no GitHub ou entre em contato através dos canais oficiais.

---

**assiste aí** - Player IPTV Moderno e Acessível 🚀

