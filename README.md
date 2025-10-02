# Sistema de Geração de Convites CRO/RS

Sistema profissional para criação de convites personalizados para eventos do Conselho Regional de Odontologia do Rio Grande do Sul.

## 🎯 Características Principais

- **4 Modelos de Convite**: Formal, Moderno, Clássico e Minimalista
- **Editor Interativo**: Prévia em tempo real das alterações
- **Gerenciamento de Convidados**: Sistema completo para cadastro e controle de remidos, autoridades e homenageados
- **Importação de Dados**: Suporte a Excel (.xlsx, .xls) e CSV para importação em massa
- **Múltiplas Opções de Exportação**: PDF, PNG, WhatsApp, E-mail e Impressão
- **QR Code**: Geração automática de QR Code para confirmação de presença
- **Design Responsivo**: Funciona perfeitamente em desktop e mobile
- **Interface Moderna**: Design profissional com paleta de cores sóbria

## 🚀 Como Usar

### Criação de Convites

1. Abra o arquivo `index.html` em um navegador
2. Clique em "Criar Convite"
3. Escolha um modelo
4. Preencha os dados do evento
5. Baixe, compartilhe ou imprima

### Gerenciamento de Convidados

1. Clique em "Gerenciar Convidados Especiais"
2. Escolha a categoria (Remidos, Autoridades ou Honra ao Mérito)
3. Cadastre manualmente ou importe de arquivo Excel/CSV
4. Acompanhe status de envio e confirmação

### Importação de Dados

Para importar listas de convidados:

1. Prepare um arquivo Excel (.xlsx, .xls) ou CSV (.csv)
2. Use o template de exemplo como referência ([template_remidos.csv](template_remidos.csv))
3. Clique em "📊 Importar Lista em Excel/CSV"
4. Selecione seu arquivo
5. Os dados serão importados automaticamente

**Campos para Remidos:**
- nome (obrigatório)
- cro (obrigatório)  
- CATEGORIA (opcional: Científica, Política, Social, Outro)
- telefone (opcional)
- email (opcional)
- NASCIMENTO (opcional, formato: AAAA-MM-DD ou DD/MM/AAAA)
- ENDEREÇO (opcional)

Para mais detalhes sobre importação, veja [IMPORT_TEMPLATE_README.md](IMPORT_TEMPLATE_README.md)

## 📋 Requisitos

- Navegador moderno (Chrome, Firefox, Safari, Edge)
- Conexão com internet (para fontes e bibliotecas externas)

## 🎨 Modelos Disponíveis

### Formal
Elegante e tradicional, com bordas douradas e linha tracejada interna.

### Moderno
Design limpo e contemporâneo com borda azul e detalhes dourados.

### Clássico
Sofisticado e atemporal com borda dupla dourada e fundo vintage.

### Minimalista
Simples e direto, focado no conteúdo.

## 📦 Tecnologias

- HTML5
- CSS3
- JavaScript (Vanilla)
- Google Fonts (Inter, Roboto)
- QRCode.js
- html2canvas
- jsPDF
- SheetJS (XLSX) - para importação de Excel/CSV

## 📖 Documentação Completa

Veja [FEATURES.md](FEATURES.md) para documentação detalhada de todas as funcionalidades.

## 📄 Licença

Sistema desenvolvido para uso do CRO/RS.
