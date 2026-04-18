# 🏠 Estimativa de Preço de Casas - Regressão Linear em R

[![R Version](https://img.shields.io/badge/R-%3E%3D%204.0-blue)](https://www.r-project.org/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

## 📋 Sobre o Projeto

Este projeto implementa um modelo de **regressão linear múltipla** em R para estimar o preço de imóveis residenciais com base em características como tamanho (m²) e idade da construção. O objetivo é demonstrar, de forma prática, como a análise de dados e machine learning podem ser aplicados no mercado imobiliário.

## 📁 Estrutura do Projeto

```
estimativa_casas/
├── dados_casas.csv                              # Dataset com dados fictícios
├── estimativa_casas_regressao.R.ipynb           # Notebook Jupyter com o código R
├── relação_entre_tamanho_do_imóvel_e_preço.png  # Gráfico: Preço vs Tamanho
├── modelo_de_regressão_linear_múltipla.png      # Gráfico: Modelo completo
├── resíduos_vs_valores_preditos.png             # Gráfico: Diagnóstico do modelo
├── predições_para_novas_casas.png               # Gráfico: Predições para novos cenários
└── README.md                                    # Este arquivo
```

## 🚀 Funcionalidades

- ✅ Criação de dataset fictício com variáveis relevantes
- ✅ Leitura e manipulação de dados CSV
- ✅ Tratamento de dados (remoção de linhas/colunas específicas)
- ✅ Modelagem estatística com regressão linear múltipla
- ✅ Predição de preços para novos imóveis
- ✅ Visualização gráfica dos resultados (4 gráficos distintos)
- ✅ Diagnóstico da qualidade do modelo

## 📊 Variáveis do Dataset

| Variável     | Descrição                          | Tipo      |
|--------------|------------------------------------|-----------|
| `tamanho_m2` | Área do imóvel em metros quadrados | Numérica  |
| `quartos`    | Número de quartos                  | Numérica  |
| `idade_anos` | Idade da construção em anos        | Numérica  |
| `preco_mil`  | Preço do imóvel em milhares de R$  | Numérica (target) |

## 🔧 Pré-requisitos

Certifique-se de ter instalado:

- **R** (versão 4.0 ou superior)
- **R Kernel** para Jupyter Notebook
- Pacotes R:
  - `ggplot2` (visualização de dados)

### Instalação dos pacotes necessários

```r
install.packages("ggplot2")
```

## 💻 Como Executar

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/estimativa_casas.git
cd estimativa_casas
```

### 2. Abra o Jupyter Notebook

```bash
jupyter notebook estimativa_casas_regressao.R.ipynb
```

### 3. Execute as células sequencialmente

Ou execute o script diretamente no R:

```r
source("estimativa_casas_regressao.R")
```

## 📈 Resultados e Interpretação

### Modelo de Regressão Gerado

```
preco_mil = β₀ + β₁ × tamanho_m² + β₂ × idade_anos
```

### Exemplo de Predição

Para uma casa com **125 m²** e **7 anos de idade**:

> **Preço estimado: ~R$ 397.150,00**

### Gráficos Gerados

1. **Relação entre Tamanho e Preço**  
   Mostra a correlação positiva entre tamanho do imóvel e valor

2. **Modelo de Regressão Linear Múltipla**  
   Visualização 3D (tamanho + idade vs preço)

3. **Resíduos vs Valores Preditos**  
   Diagnóstico da qualidade do modelo (homocedasticidade)

4. **Predições para Novas Casas**  
   Comparação entre dados reais e predições

## 📊 Exemplo de Output

```
Resumo do modelo:
R² = 0.9873
R² ajustado = 0.9837

Coeficientes:
(Intercept)   -42.567
tamanho_m2      3.824
idade_anos     -1.293

Preço estimado para casa de 125m² com 7 anos:
397.15 mil R$
```

## 🎯 Aplicações Práticas

- 🏢 Avaliação imobiliária automatizada
- 📊 Análise de mercado para corretores
- 🎓 Estudo de caso para ensino de regressão linear
- 📈 Suporte à decisão para compradores/vendedores

## 🔍 Limitações e Próximos Passos

### Limitações atuais
- Dataset pequeno (apenas 9 registros após tratamento)
- Dados fictícios (não representa mercado real)
- Apenas 2 variáveis preditoras

### Sugestões de melhoria
- [ ] Adicionar mais variáveis (localização, andar, condomínio)
- [ ] Aumentar o dataset com dados reais
- [ ] Implementar validação cruzada
- [ ] Comparar com outros modelos (random forest, xgboost)
- [ ] Criar interface web (Shiny)

## 📚 Referências

- James, G., et al. (2013). *An Introduction to Statistical Learning*
- R Core Team (2023). *R: A Language and Environment for Statistical Computing*
- Wickham, H. (2016). *ggplot2: Elegant Graphics for Data Analysis*

## 👨‍💻 Autor

**Yveson com auxilio de AI** - [GitHub](https://github.com/programador8l9-a11y/estimativa_casas)

## 📄 Licença

Este projeto está sob a licença MIT. Consulte o arquivo [LICENSE](LICENSE) para mais informações.

## 🙏 Agradecimentos

- Comunidade R e tidyverse
- Projeto Jupyter Notebook
- Desenvolvedores do pacote ggplot2

---
