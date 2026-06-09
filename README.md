# EduAtlas

## Plataforma Inteligente para Formulação, Priorização e Avaliação de Políticas Educacionais Baseadas em Evidências Territoriais

### Projeto de Pesquisa, Desenvolvimento e Inovação (PD&I)

---

# 1. Resumo Executivo

O projeto GeoEduAI propõe o desenvolvimento de uma plataforma inteligente para apoio à formulação, priorização e monitoramento de políticas públicas educacionais, integrando Inteligência Artificial, Ciência de Dados, Estatística Espacial e Sistemas de Informação Geográfica.

A solução utilizará fundamentos metodológicos derivados da metodologia SANDRA para identificar fatores críticos que influenciam indicadores educacionais em diferentes territórios, permitindo compreender não apenas os resultados observados, mas também suas causas estruturais e espaciais.

A plataforma fornecerá diagnósticos automáticos, modelos preditivos, mecanismos de recomendação de políticas públicas e ferramentas de otimização de investimentos educacionais, apoiando gestores públicos na tomada de decisão baseada em evidências.

---

# 2. Contextualização

O planejamento educacional brasileiro ainda é fortemente baseado em indicadores agregados e análises descritivas, frequentemente incapazes de capturar as diferenças territoriais que influenciam os resultados educacionais.

Municípios com indicadores semelhantes podem demandar estratégias completamente distintas devido às suas características sociais, econômicas, geográficas e institucionais.

Ao mesmo tempo, a crescente disponibilidade de bases públicas de dados educacionais e socioeconômicos cria oportunidades para o desenvolvimento de ferramentas inteligentes capazes de apoiar decisões mais precisas e efetivas.

Nesse contexto, torna-se necessário desenvolver soluções tecnológicas capazes de:

* Integrar grandes volumes de dados educacionais;
* Identificar fatores territoriais críticos;
* Detectar padrões espaciais;
* Prever cenários futuros;
* Recomendar políticas públicas;
* Apoiar a alocação eficiente de recursos.

---

# 3. Problema de Pesquisa

Como apoiar gestores públicos na formulação e priorização de políticas educacionais utilizando evidências territoriais obtidas por meio de inteligência artificial, análise espacial e modelos prescritivos?

---

# 4. Hipótese

A utilização integrada de análise espacial, inteligência artificial e identificação de variáveis territoriais críticas permite produzir recomendações de políticas públicas educacionais mais eficazes do que abordagens baseadas exclusivamente em análises estatísticas tradicionais.

---

# 5. Objetivo Geral

Desenvolver uma plataforma inteligente de apoio à decisão para formulação e priorização de políticas educacionais baseada em evidências territoriais.

---

# 6. Objetivos Específicos

## OE1

Construir um Data Lake Educacional georreferenciado.

## OE2

Integrar bases educacionais, socioeconômicas e territoriais.

## OE3

Implementar o motor analítico baseado na metodologia SANDRA.

## OE4

Desenvolver modelos preditivos de indicadores educacionais.

## OE5

Implementar mecanismos de análise espacial.

## OE6

Desenvolver um sistema de recomendação de políticas públicas.

## OE7

Implementar um módulo de otimização multiobjetivo para priorização de investimentos.

## OE8

Validar a solução em ambientes reais de gestão educacional.

---

# 7. Fundamentação Tecnológica

O projeto integra conhecimentos das áreas de:

* Inteligência Artificial
* Ciência de Dados
* Estatística Espacial
* Geoprocessamento
* Sistemas de Apoio à Decisão
* Learning Analytics
* GovTech
* EdTech
* Otimização Multiobjetivo

---

# 8. Arquitetura da Solução

```text
                 ┌──────────────────────┐
                 │ Fontes de Dados      │
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │ Data Lake Educacional│
                 └──────────┬───────────┘
                            │
                            ▼
                 ┌──────────────────────┐
                 │ Motor Analítico      │
                 │ SANDRA               │
                 └──────────┬───────────┘
                            │
      ┌─────────────────────┼─────────────────────┐
      ▼                     ▼                     ▼
 IA Preditiva       Estatística Espacial      SIG
      │                     │                     │
      └─────────────────────┼─────────────────────┘
                            ▼
                 ┌──────────────────────┐
                 │ Motor Prescritivo    │
                 └──────────┬───────────┘
                            ▼
                 ┌──────────────────────┐
                 │ Dashboards e APIs    │
                 └──────────────────────┘
```

---

# 9. Fontes de Dados

## Educação

* Censo Escolar
* IDEB
* SAEB
* ENEM
* Indicadores Educacionais do INEP

## Socioeconômicas

* IBGE
* PNUD
* IPEA

## Territoriais

* Malhas municipais
* Infraestrutura urbana
* Dados geoespaciais públicos

## Governamentais

* MEC
* Secretarias Estaduais
* Secretarias Municipais

---

# 10. Módulos Tecnológicos

## Módulo 1 – Data Lake Educacional

Responsável pela coleta, integração e armazenamento dos dados.

### Funcionalidades

* ETL automatizado
* Georreferenciamento
* Catálogo de dados
* APIs de integração

---

## Módulo 2 – Motor Analítico SANDRA

Responsável pela identificação de fatores críticos.

### Técnicas

* Correlação
* Regressão
* Seleção de atributos
* Estabilidade de variáveis
* Variabilidade regional

### Resultados

* Ranking de fatores
* Variáveis críticas
* Indicadores territoriais

---

## Módulo 3 – Inteligência Artificial

### Modelos

* Random Forest
* XGBoost
* LightGBM
* Redes Neurais

### Objetivos

* Predição do IDEB
* Predição de evasão
* Predição de proficiência
* Predição de fluxo escolar

---

## Módulo 4 – Estatística Espacial

### Técnicas

* Moran Global
* Moran Local (LISA)
* Getis-Ord
* Spatial Lag
* Spatial Error

### Produtos

* Mapas de clusters
* Hotspots educacionais
* Regiões prioritárias

---

## Módulo 5 – Sistema Prescritivo

Transformação de diagnósticos em recomendações.

### Exemplos

* Formação docente
* Conectividade escolar
* Infraestrutura
* Transporte escolar
* Permanência estudantil

---

## Módulo 6 – Otimização Multiobjetivo

### Objetivos

Maximizar:

* Aprendizagem
* Proficiência
* Equidade

Minimizar:

* Evasão
* Desigualdade territorial
* Custos

### Algoritmos

* NSGA-III
* MOEA/D
* RVEA
* NSGA-II

---

# 11. Inovação

O diferencial da proposta está na combinação de:

* Inteligência Artificial;
* Estatística Espacial;
* Sistemas Prescritivos;
* Otimização Multiobjetivo;
* Evidências Territoriais.

A solução transcende a análise descritiva tradicional ao incorporar capacidades de previsão, recomendação e simulação de cenários.

---

# 12. Produtos Tecnológicos

## Produto 1

Plataforma GeoEduAI.

## Produto 2

Motor Analítico SANDRA-Edu.

## Produto 3

Motor Prescritivo de Políticas Educacionais.

## Produto 4

API de Inteligência Territorial Educacional.

## Produto 5

Biblioteca de algoritmos de otimização para educação.

---

# 13. Resultados Esperados

* Plataforma operacional em ambiente web;
* Redução da subjetividade na tomada de decisão;
* Identificação de fatores territoriais críticos;
* Priorização inteligente de investimentos;
* Apoio à formulação de políticas públicas;
* Transferência tecnológica para órgãos públicos.

---

# 14. Formação de Recursos Humanos

## Pós-Graduação

* 1 Doutorado
* 2 Mestrados

## Graduação

* Bolsistas de Iniciação Científica

## Capacitação

* Formação de gestores públicos
* Formação de pesquisadores
* Formação de desenvolvedores

---

# 15. Cronograma (36 meses)

| Atividade                  | 1-6 | 7-12 | 13-18 | 19-24 | 25-30 | 31-36 |
| -------------------------- | --- | ---- | ----- | ----- | ----- | ----- |
| Revisão e especificação    | X   |      |       |       |       |       |
| Integração de dados        | X   | X    |       |       |       |       |
| Desenvolvimento SANDRA-Edu |     | X    | X     |       |       |       |
| IA preditiva               |     |      | X     | X     |       |       |
| Estatística espacial       |     |      | X     | X     |       |       |
| Sistema prescritivo        |     |      |       | X     | X     |       |
| Otimização multiobjetivo   |     |      |       | X     | X     |       |
| Pilotos                    |     |      |       |       | X     |       |
| Transferência tecnológica  |     |      |       |       |       | X     |

---

# 16. Potencial de Enquadramento na Lei de Informática

O projeto apresenta aderência às diretrizes da Lei de Informática por envolver:

* Pesquisa aplicada;
* Desenvolvimento de software inovador;
* Inteligência Artificial;
* Ciência de Dados;
* Formação de recursos humanos;
* Transferência tecnológica;
* Cooperação entre empresas e ICTs;
* Geração de propriedade intelectual.

Além disso, produz ativos tecnológicos passíveis de exploração comercial e transferência para organizações públicas e privadas.
