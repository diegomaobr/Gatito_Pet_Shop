# Power BI Report Project

Este repositório contém a estrutura descompactada de um relatório e painel interativo do **Power BI**, incluindo seu modelo de dados (`DataModel`), layouts de página e visuais customizados (*Custom Visuals*).

---

## 📊 Estrutura do Projeto

A organização dos arquivos e pastas no repositório reflete a estrutura interna do arquivo do Power BI:

```text
.
├── DataModel                                   # Modelo de dados comprimido (tabelas, relacionamentos e medidas)
├── SecurityBindings                             # Configurações de segurança e permissões
├── [Content_Types].xml                         # Mapeamento dos tipos de conteúdo do arquivo
├── Version                                     # Versão do formato de arquivo do Power BI
├── Report/
│   ├── definition/                             # Definições de layout, páginas e visuais em JSON
│   │   ├── report.json                         # Configurações gerais do relatório
│   │   ├── version.json                        # Versão do esquema do relatório
│   │   └── pages/                              # Configuração estrutural das páginas e visuais (Desktop e Mobile)
│   ├── CustomVisuals/                          # Visuais customizados importados para o projeto
│   │   ├── ImageGrid/                          # Visual personalizado para exibição de imagens em grade
│   │   ├── textFilter/                         # Filtro de texto avançado
│   │   ├── textfromval/                        # Visual para manipulação de valores de texto
│   │   └── textSearchSlicer/                   # Segmentador de busca por texto
│   └── StaticResources/                        # Recursos estáticos (temas e imagens)
│       ├── RegisteredResources/                # Imagens registradas no relatório (ex: Gatito.jpg)
│       └── SharedResources/BaseThemes/         # Tema base aplicado (ex: CY24SU06.json)
```

---

## 🛠️ Visuais Customizados (Custom Visuals)

Este projeto utiliza suplementos de visuais personalizados para enriquecer a experiência de análise:

* **Text Filter** (`textFilter25A4896A83E0487089E2B90C9AE57C8A`): Permite filtragem direta de campos de texto.
* **Text Search Slicer** (`textSearchSlicerF85E2E78BE4A4D7D9F99ED75B5D71C85`): Segmentador com pesquisa rápida em tabelas de dados.
* **Text From Val** (`textfromval067F5682FE6D4A43B334273EA44AE0EB`): Componente para formatação dinâmica de texto baseada em valores.
* **Image Grid** (`ImageGrid_FC5183B9_926C_45E0_B5F7_0CE9EAF1DA9B`): Exibição de imagens vinculadas aos dados em formato de grade.

---

## 🚀 Como Utilizar

### 1. Compactar para arquivo `.pbix`
Para abrir este relatório diretamente no **Power BI Desktop**:

1. Selecione todos os arquivos e pastas da raiz do projeto.
2. Compacte-os em formato `.zip`.
3. Renomeie a extensão do arquivo final de `.zip` para `.pbix`.
4. Abra o arquivo `.pbix` no **Power BI Desktop**.

> **Nota:** Certifique-se de compactar o conteúdo **diretamente na raiz** do arquivo ZIP (sem criar uma pasta pai dentro do ZIP).

---

## 💻 Requisitos

* **Power BI Desktop** (versão recomendada: 2024 ou superior).
* Acesso às fontes de dados configuradas no modelo.

---

## 📝 Licença e Contribuição

Contribuições para melhorias no layout, otimização de DAX ou ajustes no modelo de dados são bem-vindas. Sinta-se à vontade para abrir uma *Issue* ou enviar um *Pull Request*.