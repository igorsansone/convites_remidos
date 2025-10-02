# Template de Importação de Remidos

Este arquivo serve como exemplo para importação de dados de remidos no sistema de gerenciamento de convidados CRO/RS.

## Formatos Aceitos

- **Excel**: .xlsx, .xls
- **CSV**: .csv

## Estrutura do Arquivo

O arquivo deve conter as seguintes colunas (os nomes podem variar, o sistema reconhece automaticamente):

| Campo | Nomes Aceitos | Obrigatório | Exemplo |
|-------|---------------|-------------|---------|
| Nome | nome, name | ✅ Sim | João da Silva |
| CRO | cro, nº cro, numero cro, cro/rs | ✅ Sim | 12345 |
| Categoria | categoria, category | ⚪ Opcional | Científica, Política, Social, Outro |
| Telefone | telefone, telefone celular, celular, phone, tel | ⚪ Opcional | (51) 99999-9999 |
| E-mail | email, e-mail, mail | ⚪ Opcional | exemplo@email.com |
| Nascimento | nascimento, data de nascimento, birth, birthday | ⚪ Opcional | 1980-01-15 ou 15/01/1980 |
| Endereço | endereço, endereco, address, rua | ⚪ Opcional | Rua Exemplo, 123 - Centro - Porto Alegre/RS |

## Formato de Data

As datas de nascimento podem ser informadas em diversos formatos:
- ISO: `1980-01-15`
- Brasileira: `15/01/1980`
- Americana: `01/15/1980`
- Número do Excel (será convertido automaticamente)

## Categorias Válidas

- **Científica** (ou científico, cientifica)
- **Política** (ou político, politica)
- **Social**
- **Outro** (ou other)

## Como Usar

1. Use o arquivo `template_remidos.csv` como exemplo
2. Preencha com seus dados seguindo a estrutura
3. No sistema, vá em **Gerenciar Convidados Especiais** > **Remidos**
4. Clique em **Importar Lista em Excel/CSV**
5. Selecione seu arquivo
6. Os dados serão importados automaticamente

## Observações

- Campos obrigatórios: **nome** e **cro**
- O sistema é flexível com os nomes das colunas (case-insensitive)
- Linhas vazias serão ignoradas
- Erros de importação serão exibidos ao final do processo
- Você pode usar o botão "⬇️ Baixar modelo de exemplo" no sistema para gerar templates automaticamente

## Exemplo de CSV

```csv
nome,cro,CATEGORIA,telefone,email,NASCIMENTO,ENDEREÇO
João da Silva,12345,Científica,(51) 99999-9999,joao@example.com,1980-01-15,"Rua Exemplo, 123 - Centro - Porto Alegre/RS"
Maria Santos,67890,Social,(51) 98888-8888,maria@example.com,1985-05-20,"Av. Protásio Alves, 456 - Petrópolis - Porto Alegre/RS"
```

## Suporte

Em caso de dúvidas sobre a importação, verifique:
1. Se o arquivo está no formato correto (.xlsx, .xls ou .csv)
2. Se as colunas obrigatórias (nome e cro) estão presentes
3. Se não há caracteres especiais problemáticos
4. A mensagem de erro exibida pelo sistema indicará a linha e o problema específico
