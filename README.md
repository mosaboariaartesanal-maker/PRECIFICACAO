# Sistema de Precificação – MÔ SABOARIA

Sistema web desenvolvido para auxiliar no gerenciamento de custos, controle de ingredientes, elaboração de fichas técnicas e formação de preços de venda dos produtos artesanais da **MÔ SABOARIA**.

A aplicação permite organizar informações financeiras e produtivas, automatizar cálculos de precificação e acompanhar indicadores importantes para a tomada de decisões comerciais.

## 1. Funcionalidades

### Dashboard
Painel principal com indicadores e gráficos para acompanhamento do desempenho financeiro e dos produtos cadastrados.

- Quantidade de produtos cadastrados.
- Preço médio de revenda.
- Total de despesas fixas.
- Margem de contribuição média.
- Ponto de equilíbrio em produtos.
- Faturamento necessário para cobrir as despesas fixas.
- Análise individual dos produtos.
- Gráfico dos cinco produtos com maior margem de contribuição.
- Gráfico de despesas fixas por categoria.
- Gráfico dos cinco produtos com maiores custos.
- Comparativo entre faturamento e despesas fixas.

### Custos e Taxas
Área destinada ao cadastro e gerenciamento das despesas necessárias para manter a operação.

- Cadastro e exclusão de custos fixos.
- Descrição e classificação das despesas por categoria.
- Cálculo automático do total de despesas fixas.
- Cadastro do faturamento médio mensal.
- Cálculo do percentual de custos fixos sobre o faturamento.
- Gerenciamento de categorias de despesas.

### Fichas Técnicas e Precificação
Módulo responsável pela composição dos produtos e formação automatizada dos preços de venda.

- Cadastro e edição de produtos.
- Inclusão e exclusão de ingredientes nas fichas técnicas.
- Definição do rendimento de cada ficha.
- Cálculo automático do custo total dos ingredientes.
- Cálculo do custo de insumos por unidade produzida.
- Distribuição proporcional dos custos fixos.
- Inclusão de custos de embalagem.
- Definição do markup desejado.
- Inclusão de impostos e taxas de cartão.
- Inclusão de taxas de delivery/iFood.
- Cálculo do preço de venda com markup.
- Cálculo do preço sugerido de venda.
- Registro do preço efetivamente praticado.
- Cálculo do markup aplicado.
- Identificação de produtos que precisam de ajustes na precificação.
- Cálculo da margem de contribuição.
- Geração de fichas técnicas em PDF.

### Cadastro de Ingredientes
Módulo para gerenciamento dos insumos utilizados na fabricação dos produtos.

- Cadastro de ingredientes.
- Edição das informações cadastradas.
- Exclusão de ingredientes.
- Definição da unidade de medida.
- Registro da quantidade adquirida.
- Registro do valor de compra.
- Cálculo automático do custo unitário.
- Pesquisa de ingredientes cadastrados.
- Integração com as fichas técnicas.

## 2. Tecnologias utilizadas

O sistema foi desenvolvido utilizando tecnologias web:

- **HTML5:** estrutura e organização da aplicação.
- **CSS3:** estilização, layout responsivo e temas visuais.
- **JavaScript:** funcionalidades, cálculos automáticos, gerenciamento de dados e interatividade.
- **Chart.js:** criação dos gráficos do Dashboard.
- **jsPDF:** geração de documentos PDF das fichas técnicas.
- **LocalStorage:** armazenamento local dos dados no navegador.

## 3. Estrutura do sistema

O sistema está organizado em quatro módulos principais:

| Módulo | Finalidade |
|---|---|
| Dashboard | Indicadores e gráficos gerenciais |
| Custos e Taxas | Gerenciamento das despesas e faturamento |
| Fichas Técnicas | Composição dos produtos e precificação |
| Ingredientes | Cadastro e gerenciamento de insumos |

## 4. Fórmulas e cálculos

O sistema utiliza fórmulas automatizadas para auxiliar na formação dos preços.

**Custo unitário do ingrediente:**

Valor de compra ÷ Quantidade comprada.

**Custo total da ficha técnica:**

Soma dos custos de todos os ingredientes utilizados.

**Custo de insumos por unidade:**

Custo total da ficha técnica ÷ Rendimento da ficha.

**Percentual de custos fixos:**

Total de despesas fixas ÷ Faturamento médio mensal.

**Custo fixo por produto:**

Custo de insumos por unidade × Percentual de custos fixos.

**Custo total do produto:**

Custo de insumos + Custo fixo + Embalagem.

**Preço com markup:**

Custo total × (1 + Markup desejado).

**Preço sugerido de venda:**

Preço com markup ÷ (1 − Percentual de impostos − Taxa de cartão − Taxa de delivery/iFood).

**Margem de contribuição:**

Preço praticado − Custos totais − Taxas incidentes sobre a venda.

## 5. Como utilizar

1. Baixe o arquivo HTML do sistema.
2. Abra o arquivo utilizando um navegador atualizado, como Google Chrome, Microsoft Edge ou Firefox.
3. Acesse a aba **Ingredientes** e confira ou cadastre os insumos utilizados na produção.
4. Acesse **Custos e Taxas** e informe as despesas fixas e o faturamento médio mensal.
5. Entre em **Fichas Técnicas** e cadastre os produtos, seus ingredientes, quantidades e rendimento.
6. Informe os valores de embalagem, markup, impostos e taxas aplicáveis.
7. Consulte os preços sugeridos e as margens de contribuição.
8. Utilize o Dashboard para acompanhar os indicadores.
9. Gere PDFs das fichas técnicas quando necessário.

## 6. Armazenamento de dados

O sistema utiliza o LocalStorage do navegador para armazenar as informações cadastradas.

Isso significa que:

- Os dados ficam salvos no navegador utilizado.
- As alterações são armazenadas automaticamente.
- Fechar o navegador não apaga os dados.
- Acessar o sistema em outro computador ou navegador não transfere automaticamente os dados.
- Limpar os dados do navegador pode apagar os registros armazenados.

**Recomendação:** mantenha cópias de segurança dos dados. O código atual não implementa sincronização em nuvem nem um mecanismo próprio de exportação e restauração dos cadastros.

## 7. Observações técnicas

- A interface possui layout responsivo para computadores, tablets e dispositivos móveis.
- Disponibiliza alternância entre tema claro e escuro.
- Os cálculos são atualizados conforme as informações cadastradas.
- Os gráficos são construídos a partir dos indicadores calculados.
- A geração de PDF possui alternativa de impressão e salvamento como PDF pelo navegador.
- O sistema utiliza bibliotecas externas carregadas por CDN, sendo necessário acesso à internet para disponibilizá-las quando não estiverem em cache.

## 8. Objetivo do projeto

O Sistema de Precificação MÔ SABOARIA tem como finalidade proporcionar maior organização, controle e precisão na gestão dos custos de fabricação e na formação dos preços dos produtos artesanais.

A ferramenta busca facilitar o acompanhamento dos gastos, identificar os custos reais de produção e auxiliar na definição de preços de venda mais adequados, contribuindo para uma gestão comercial mais organizada e sustentável.

---

**Projeto:** Sistema de Precificação MÔ SABOARIA  
**Tipo:** Aplicação Web  
**Formato:** HTML, CSS e JavaScript  
**Armazenamento:** LocalStorage  
**Idioma:** Português (Brasil)
