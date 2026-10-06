# Projeto-DIO-Imposto-de-Renda
App construído no Excel para simular entradas de um Imposto de Renda
# Fox Taxes: Agregador Inteligente de Imposto de Renda

Um sistema de gestão financeira e validação de dados desenvolvido no Excel, projetado com uma interface *Premium*. A ferramenta centraliza, categoriza e valida o fluxo de informações necessárias para a declaração do Imposto de Renda, funcionando como um verdadeiro aplicativo.

## Objetivo e Motivação
Este projeto foi desenvolvido como parte de um desafio da **DIO**, mas a sua arquitetura foi inteiramente baseada em desafios reais do mercado de trabalho. A motivação surgiu da necessidade prática de otimizar rotinas complexas de conciliação financeira.

O objetivo principal foi abandonar planilhas rudimentares e criar um sistema escalável, garantindo:
1. Padronização na entrada de dados para mitigar erros e riscos de malha fina.
2. Agrupamento lógico de despesas dedutíveis e rendimentos tributáveis.
3. Interface intuitiva que reduz a fadiga visual durante o preenchimento de grandes volumes de informações.

## Funcionalidades e UI/UX
A identidade visual da **Fox Taxes** utiliza tons em contrastes em laranja, transmitindo segurança, agilidade e inteligência estratégica:

* **Registro Geral de Movimentos :** O sistema utiliza uma arquitetura de banco de dados unificado. Entradas (Receitas) e Saídas (Despesas) convivem na mesma tabela inteligente, o que simplifica drasticamente a futura geração de relatórios com Tabelas Dinâmicas ou funções `SOMASES`.
* **Estrutura de Colunas:** O registro exige o preenchimento estruturado de `Data`, `Movimentação` (Entrada/Saída), `Nº NF/DOC`, `Categoria` (via validação), `Valor` e `Descrição` (texto livre para colocar qualquer informação).
* **Menu de Navegação Interativo:** Um *dashboard* inicial limpo, com botões que guiam o usuário de forma fluida pelas funcionalidades.

## Estrutura Técnica e Back-end
* **Validação de Dados Estrita:** Controle rigoroso da coluna de "Categorias", alimentada por uma base de apoio. As opções refletem exatamente os campos do programa oficial da Receita Federal (ex: *Salário / Pró-Labore, Despesa Médica / Saúde, Despesa de Custeio, Lucros e Dividendos*).
* **Camada de Apoio Oculta:** Separação entre a interface do usuário e as listas de categorias e parâmetros. As abas de base são ocultadas para proteger a integridade do sistema.
* **Hiperlinks Internos:** Roteamento dentro do próprio documento para criar uma experiência de navegação ágil.

## 📸 Demonstração da Interface

### 1. Menu de Navegação Principal
<img width="257" height="925" alt="image" src="https://github.com/user-attachments/assets/9dbce6a1-f446-4cdb-855d-95e3cf2f8f06" />

### 2. Módulo de Registro de Movimentações
<img width="1328" height="870" alt="image" src="https://github.com/user-attachments/assets/96e0bf65-cf57-46a4-8964-aebac9f01813" />
---
**Ferramentas Utilizadas:** Microsoft Excel, GitHub.
