# Sistema Profissional de Geração de Convites CRO/RS

## Visão Geral
Sistema completo e profissional para criação de convites personalizados para eventos do CRO/RS (Conselho Regional de Odontologia do Rio Grande do Sul).

## Recursos Principais

### 1. Tela de Boas-Vindas
- Design moderno com gradiente azul escuro profissional
- Logo do CRO/RS em destaque
- Descrição clara do sistema
- Botão "Criar Convite" com animações e efeitos hover

### 2. Editor de Convites Interativo

#### Seleção de Modelos
O sistema oferece **4 modelos diferentes** de convite:

1. **Formal**: Elegante e tradicional
   - Bordas douradas em gradiente
   - Linha tracejada interna decorativa
   - Ideal para solenidades e eventos oficiais

2. **Moderno**: Limpo e contemporâneo
   - Borda azul escuro à esquerda
   - Fundo com gradiente sutil
   - Detalhes em dourado
   - Perfeito para eventos modernos

3. **Clássico**: Sofisticado e atemporal
   - Borda dupla dourada
   - Fundo em tom creme vintage
   - Estilo tradicional e elegante

4. **Minimalista**: Simples e direto
   - Borda simples e discreta
   - Design limpo e objetivo
   - Foco no conteúdo

#### Campos Customizáveis
- **Tipo de Evento**: Solenidade, Reunião, Comemoração ou Outro
- **Nome do Convidado**: Campo de texto livre
- **Data do Evento**: Texto personalizável (ex: "15 de dezembro de 2024")
- **Local do Evento**: Endereço ou nome do local
- **Horário**: Horário do evento
- **Mensagem Personalizada**: Campo opcional para mensagens especiais

#### Opções Adicionais
- **QR Code**: Opção para incluir QR Code no convite
  - Campo para inserir link de confirmação de presença
  - QR Code gerado automaticamente
  - Exibido no rodapé do convite com label "Escaneie para confirmar presença"

### 3. Prévia em Tempo Real
- Atualização instantânea ao digitar
- Visualização exata do convite final
- Troca dinâmica entre modelos
- Placeholder inteligente para campos vazios

### 4. Ações Disponíveis

#### 📄 Baixar PDF
- Converte o convite para PDF de alta qualidade
- Formato A4 otimizado para impressão
- Utiliza jsPDF para geração

#### 🖼️ Baixar Imagem
- Salva o convite como imagem PNG
- Alta resolução (2x scale)
- Ideal para compartilhamento digital

#### 📱 WhatsApp
- Compartilhamento direto via WhatsApp
- Mensagem pré-formatada com todos os detalhes do evento
- Abre o WhatsApp Web ou aplicativo automaticamente

#### 📧 E-mail
- Abre cliente de e-mail padrão
- Assunto e corpo pré-preenchidos
- Mensagem formal e profissional

#### 🖨️ Imprimir
- Função de impressão otimizada
- Remove elementos de interface (formulário, botões)
- Mantém apenas o convite para impressão limpa

## Design e Estética

### Paleta de Cores
- **Azul Escuro**: #1a237e, #283593 (principal)
- **Branco**: #ffffff (fundo)
- **Cinza**: #f5f7fa, #e0e0e0 (elementos secundários)
- **Dourado**: #d4af37, #f4d03f (destaques e acentos)
- **Azul Claro**: #5c6bc0 (subtítulos)

### Tipografia
- **Fontes Principais**: Inter, Roboto
- **Peso**: 400 (regular), 500 (medium), 600 (semibold), 700 (bold)
- **Estilo**: Moderno, limpo e profissional

### Elementos de Interface
- Bordas arredondadas (8px-16px)
- Sombras suaves para profundidade
- Transições suaves (0.3s)
- Efeitos hover interativos
- Layout espaçado e respirável

## Responsividade

### Desktop (> 968px)
- Layout de duas colunas (formulário + prévia)
- Botões de ação em 2 colunas
- Espaçamento amplo

### Mobile (≤ 968px)
- Layout de coluna única
- Botões empilhados (1 coluna)
- Otimizado para telas pequenas
- Touch-friendly

### Impressão
- Remove elementos de interface
- Mantém apenas o convite
- Otimizado para papel A4

## Tecnologias

### Frontend
- HTML5
- CSS3 (Flexbox, Grid, Gradients, Animations)
- JavaScript ES6+ (Vanilla JS)

### Bibliotecas Externas
- **Google Fonts**: Inter e Roboto
- **QRCode.js**: Geração de QR Codes
- **html2canvas**: Captura de screenshot
- **jsPDF**: Geração de PDF

## Funcionalidades Técnicas

### Gerenciamento de Estado
- Atualização de prévia em tempo real via event listeners
- Troca dinâmica de templates
- Toggle condicional de elementos (QR Code)

### Validação
- Campos opcionais claramente marcados
- Placeholders informativos
- Feedback visual para campos preenchidos

### Acessibilidade
- Labels semânticos
- Estrutura HTML adequada
- Contraste de cores apropriado
- Navegação por teclado

## Como Usar

1. **Acesse a página inicial**: Visualize a tela de boas-vindas
2. **Clique em "Criar Convite"**: Entre no editor
3. **Escolha um modelo**: Selecione entre Formal, Moderno, Clássico ou Minimalista
4. **Preencha os dados**: 
   - Selecione o tipo de evento
   - Digite nome do convidado
   - Informe data, local e horário
   - Adicione mensagem personalizada (opcional)
5. **Adicione QR Code** (opcional): Marque a opção e insira o link
6. **Visualize a prévia**: Confira em tempo real
7. **Escolha uma ação**:
   - Baixe em PDF ou PNG
   - Compartilhe via WhatsApp ou E-mail
   - Imprima diretamente

## Exemplos de Uso

### Solenidade de Posse
- Modelo: Formal
- Mensagem: Texto protocolar e oficial

### Reunião Técnica
- Modelo: Moderno ou Minimalista
- Mensagem: Objetiva e direta

### Comemoração
- Modelo: Clássico
- Mensagem: Calorosa e convidativa

## Manutenção e Extensibilidade

### Adicionar Novo Modelo
1. Adicione classe CSS `.template-[nome]`
2. Defina estilos específicos
3. Adicione opção no HTML
4. Atualize objeto `titles` no JavaScript

### Personalizar Cores
- Modifique variáveis CSS no topo do arquivo
- Atualize gradientes e cores de acento
- Mantenha contraste adequado

### Adicionar Novos Campos
1. Adicione elemento no formulário
2. Crie elemento correspondente na prévia
3. Adicione lógica no `atualizarPrevia()`
4. Adicione event listener

## Suporte e Compatibilidade

### Navegadores Suportados
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Dispositivos
- Desktop (Windows, macOS, Linux)
- Tablet (iPad, Android)
- Mobile (iOS, Android)

## Licença
Sistema desenvolvido para uso exclusivo do CRO/RS.
