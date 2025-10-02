# Changelog

## [Unreleased] - 2024-10-02

### Added - Importação de Remidos com Novos Campos

#### Novos Campos no Formulário
- Campo **Categoria** (dropdown: Científica, Política, Social, Outro)
- Campo **Data de Nascimento** (date input com formatação brasileira)
- Campo **Endereço** (text input para endereço completo)

#### Suporte a Importação CSV
- Suporte a arquivos CSV (.csv) além de Excel (.xlsx, .xls)
- Processador CSV nativo em JavaScript
- Reconhecimento inteligente de colunas (case-insensitive)
- Conversão automática de formatos de data
- Mapeamento de categorias

#### Importação Excel Aprimorada
- Processamento dos novos campos: categoria, nascimento, endereço
- Validação de campos obrigatórios (nome, cro)
- Relatório detalhado de erros de importação
- Suporte a múltiplas variações de nomes de colunas

#### Visualização Atualizada
- Tabela com 3 novas colunas: Categoria, Nascimento, Endereço
- Cards com exibição completa dos novos campos
- Formatação brasileira de datas (DD/MM/AAAA)
- Ícones apropriados para cada campo

#### Templates e Documentação
- Arquivo `template_remidos.csv` com exemplo de importação
- Documentação completa em `IMPORT_TEMPLATE_README.md`
- README.md atualizado com instruções de importação
- Botão de download de template na interface

#### Melhorias Técnicas
- Função `downloadTemplate()` para gerar templates Excel e CSV
- Parser CSV robusto com tratamento de aspas e vírgulas
- Conversão de datas do Excel (número serial)
- Tratamento de múltiplos formatos de data
- Validação e sanitização de dados

### Modified
- `index.html` - Formulário, importação, renderização de tabela e cards
- `README.md` - Documentação atualizada

### Created
- `template_remidos.csv` - Template de exemplo para importação
- `IMPORT_TEMPLATE_README.md` - Guia completo de importação
- `CHANGELOG.md` - Este arquivo

### Technical Details

#### Campos Reconhecidos na Importação

| Campo | Variações Aceitas |
|-------|-------------------|
| Nome | nome, name |
| CRO | cro, nº cro, numero cro, cro/rs |
| Categoria | categoria, category |
| Telefone | telefone, telefone celular, celular, phone, tel |
| E-mail | email, e-mail, mail |
| Nascimento | nascimento, data de nascimento, birth, birthday, data_nascimento |
| Endereço | endereço, endereco, address, rua |

#### Valores de Categoria

- **Científica**: científico, cientifica, científ, cientif
- **Política**: político, politica, polít, polit  
- **Social**: social
- **Outro**: outro, other (ou qualquer outro valor)

#### Formatos de Data Suportados

- ISO 8601: `AAAA-MM-DD` (ex: 2024-01-15)
- Brasileira: `DD/MM/AAAA` (ex: 15/01/2024)
- Americana: `MM/DD/AAAA` (ex: 01/15/2024)
- Número do Excel: Conversão automática de serial date

### Testing

✅ Testes realizados:
- Cadastro manual com novos campos
- Visualização em tabela
- Visualização em cards
- Persistência de dados (localStorage)
- Formatação de datas
- Labels de categoria
- Template CSV

### Files Changed

```
 CHANGELOG.md                   | 111 ++++++++++++++++++
 IMPORT_TEMPLATE_README.md      |  89 +++++++++++++
 README.md                      |  46 +++++++
 index.html                     | 275 +++++++++++++++++++++++++-------------
 template_remidos.csv           |   3 +
 5 files changed, 432 insertions(+), 92 deletions(-)
```

### Example Import File

```csv
nome,cro,CATEGORIA,telefone,email,NASCIMENTO,ENDEREÇO
João da Silva,12345,Científica,(51) 99999-9999,joao@example.com,1980-01-15,"Rua Exemplo, 123"
Maria Santos,67890,Social,(51) 98888-8888,maria@example.com,1985-05-20,"Av. Protásio, 456"
```

### Screenshots

- Formulário: https://github.com/user-attachments/assets/9791965c-9001-471f-8c7a-d184051b08d2
- Tabela: https://github.com/user-attachments/assets/54fd6d41-7841-402d-a08b-a926cd1422fa
- Cards: https://github.com/user-attachments/assets/c76f16dc-3561-473a-8ccb-4e801a825c96

---

## Previous Versions

### [1.0.0] - Initial Release
- Sistema de geração de convites
- Gerenciamento de convidados
- Importação Excel básica
