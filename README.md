# EduAtlas: Plataforma de Inteligência Territorial Educacional
## Projeto de Pesquisa, Desenvolvimento e Inovação (PD&I) — Lei de Informática

---

# 1. Resumo Executivo

O projeto **EduAtlas (GeoEduAI)** propõe o desenvolvimento de uma plataforma inteligente de suporte à formulação, priorização e monitoramento de políticas públicas educacionais baseadas em evidências territoriais. A solução integrará Inteligência Artificial, Ciência de Dados, Estatística Espacial e Sistemas de Informação Geográfica (SIG).

A plataforma utilizará fundamentos metodológicos derivados da **Metodologia SANDRA** para identificar de forma automatizada os fatores críticos socioeconômicos e estruturais que influenciam os indicadores educacionais em diferentes recortes geográficos. A solução transborda a análise descritiva tradicional ao fornecer diagnósticos automáticos, modelos preditivos, mecanismos de recomendação de políticas públicas e ferramentas de otimização de investimentos educacionais, apoiando gestores na tomada de decisão estratégica com foco em equidade e eficiência.

---

# 2. Contextualização e Problema de Pesquisa

O planejamento educacional e a alocação de recursos públicos no cenário brasileiro ainda dependem fortemente de indicadores estatísticos agregados (médias municipais ou estaduais). Essa abordagem descritiva tradicional falha em capturar as severas assimetrias e variabilidades territoriais que influenciam diretamente o desempenho escolar. Municípios ou escolas com indicadores de resultado idênticos frequentemente demandam intervenções estruturais completamente distintas em virtude de suas características demográficas, socioeconômicas, institucionais e de localização.

Com o aumento da maturidade digital dos órgãos governamentais e a ampla disponibilidade de bases públicas de microdados estruturados e desestruturados, surge a oportunidade tecnológica para a criação de sistemas inteligentes baseados em evidências geográficas detalhadas.

### Problema de Pesquisa
Como apoiar gestores públicos na formulação e priorização de políticas educacionais utilizando evidências territoriais obtidas por meio de inteligência artificial, análise espacial e modelos prescritivos de alocação de recursos?

### Hipótese
A utilização integrada de algoritmos de análise espacial, aprendizagem automática e isolamento estatístico de variáveis territoriais críticas permite produzir recomendações de políticas públicas educacionais mais eficazes, equitativas e preditivas do que as abordagens analíticas e estatísticas tradicionais.

---

# 3. Objetivos

## Objetivo Geral
Desenvolver uma plataforma inteligente de suporte à decisão (SaaS) para formulação, priorização e avaliação de políticas educacionais baseada em evidências territoriais.

## Objetivos Específicos (OE)
* **OE1:** Construir um Data Lake Educacional unificado e georreferenciado.
* **OE2:** Integrar e automatizar pipelines de dados estruturados e geoespaciais provenientes de bases educacionais, socioeconômicas e territoriais públicas.
* **OE3:** Implementar o motor analítico core baseado na Metodologia SANDRA para isolamento de fatores críticos e avaliação de instabilidade regional.
* **OE4:** Desenvolver e treinar modelos preditivos de inteligência artificial voltados a indicadores de proficiência, fluxo e abandono escolar.
* **OE5:** Implementar mecanismos avançados de estatística espacial para detecção de clusters e *hotspots* de vulnerabilidade.
* **OE6:** Desenvolver um sistema de recomendação prescritivo de políticas públicas baseado nas vulnerabilidades mapeadas.
* **OE7:** Implementar um módulo de otimização multiobjetivo para apoio à tomada de decisão e priorização de investimentos financeiros em educação.
* **OE8:** Validar a solução em ambientes de gestão educacional reais por meio do desenvolvimento de projetos-piloto.

---

# 4. Arquitetura da Solução e Fluxo Tecnológico

```text
                  ┌──────────────────────┐
                  │   Fontes de Dados    │
                  └──────────┬───────────┘
                             │
                             ▼
                  ┌──────────────────────┐
                  │ Data Lake Educacional│
                  └──────────┬───────────┘
                             │
                             ▼
                  ┌──────────────────────┐
                  │   Motor Analítico    │
                  │       SANDRA         │
                  └──────────┬───────────┘
                             │
      ┌─────────────────────┼─────────────────────┐
      ▼                     ▼                     ▼
 IA Preditiva      Estatística Espacial           SIG
      │                     │                     │
      └─────────────────────┼─────────────────────┘
                            ▼
                  ┌──────────────────────┐
                  │  Motor Prescritivo   │
                  │    e Otimização      │
                  └──────────┬───────────┘
                             │
                             ▼
                  ┌──────────────────────┐
                  │  Dashboards e APIs   │
                  └──────────────────────┘

---

# 5. Fontes de Dados Mapeadas

### Educação

* Censo Escolar (INEP)
* Índice de Desenvolvimento da Educação Básica (IDEB)
* Sistema de Avaliação da Educação Básica (SAEB)
* Exame Nacional do Ensino Médio (ENEM)
* Indicadores de Fluxo, Distorção Idade-Série e Taxas de Rendimento (INEP)

### Socioeconômicas

* Censo Demográfico e Estimativas Populacionais (IBGE)
* Índice de Desenvolvimento Humanano Municipal (IDHM/PNUD)
* Cadastro Único para Programas Sociais (CadÚnico) e dados de vulnerabilidade social (IPEA)

### Territoriais e Governamentais

* Malhas digitais municipais, estaduais e de setores censitários (IBGE)
* Camadas geográficas de infraestrutura de transporte, redes elétricas e conectividade telecom
* Dados de execução orçamentária obtidos via convênios com o MEC e Secretarias de Educação

---

# 6. Módulos Tecnológicos

## Módulo 1 – Data Lake Educacional

Infraestrutura de dados escalável voltada à ingestão, normalização, armazenamento e governança das bases de dados.

* **Funcionalidades:** Pipelines de ETL/ELT automatizados, rotinas de geocodificação e compatibilização de coordenadas geográficas, catálogo de metadados centralizado e barramento de APIs seguras para consumo interno e externo.

## Módulo 2 – Motor Analítico SANDRA

Módulo de processamento estatístico avançado derivado da metodologia da dissertação para identificação de correlações reais e isolamento de dependências.

* **Técnicas:** Algoritmos de seleção de atributos (*Feature Selection*), modelagem de regressão robusta, análises de estabilidade temporal e regional de variáveis independentes e quantificação de impacto local.
* **Entregas:** Criação de rankings automatizados de fatores de impacto, isolamento de variáveis críticas locais e geração de indicadores de vulnerabilidade ajustados ao território.

## Módulo 3 – Inteligência Artificial Preditiva

Subsistema focado no treinamento de modelos preditivos supervisionados de Machine Learning para simulação de cenários educacionais.

* **Modelos:** Algoritmos de aprendizado supervisionado baseados em árvores de decisão e conjuntos de modelos (*Random Forest, XGBoost, LightGBM*) e arquiteturas de Redes Neurais para dados tabulares.
* **Objetivos:** Predição de trajetórias do IDEB, classificação de risco de evasão precoce por unidade escolar, estimativa de proficiência em exames padronizados e modelagem de fluxo escolar.

## Módulo 4 – Estatística Espacial e Inteligência Geográfica

Módulo analítico que aplica algoritmos de geografia quantitativa para compreender a distribuição e a dependência espacial dos fenômenos educacionais.

* **Técnicas:** Índice de Autocorrelação Espacial de Moran Global e Local (LISA), estatística espacial de Getis-Ord ($G_i^*$), modelagem econométrica espacial (*Spatial Lag Model* — SLM e *Spatial Error Model* — SEM).
* **Produtos:** Geração dinâmica de mapas de clusters (Alto-Alto, Baixo-Baixo), detecção automatizada de *hotspots* de exclusão escolar e isolamento geográfico de regiões críticas prioritárias.

## Módulo 5 – Sistema Prescritivo e Recomendação de Políticas

Camada lógica responsável por correlacionar os diagnósticos analíticos, espaciais e preditivos com linhas de ação e intervenções pedagógicas e de infraestrutura.

* **Escopo de Recomendação:** Alocação de programas de formação continuada para docentes, direcionamento de investimentos inovações em conectividade escolar banda larga, expansão da rede de transporte escolar rural, programas de prevenção do abandono e otimização da distribuição da infraestrutura física (quadras, laboratórios, bibliotecas).

## Módulo 6 – Otimização Multiobjetivo

Algoritmo de pesquisa operacional voltado ao suporte à decisão sob restrições orçamentárias severas.

* **Funções-Objetivo (Maximizar):** Níveis gerais de aprendizagem, taxas de proficiência e equidade na distribuição de insumos entre escolas.
* **Funções-Objetivo (Minimizar):** Taxas de evasão escolar, desigualdade socioespacial intracorporativa e custos operacionais de investimento.
* **Algoritmos Aplicados:** Algoritmos genéticos evolutivos multiobjetivo (*NSGA-III, MOEA/D, RVEA, NSGA-II*).

---

# 7. Modelo Comercial (SaaS) e Camada Gratuita

A plataforma EduAtlas será comercializada sob o modelo de negócio **SaaS (Software as a Service) Fechado**, mediante a contratação de assinaturas recorrentes por órgãos públicos (Secretarias de Educação) e instituições privadas.

Para atração, experimentação técnica e disseminação da metodologia, o projeto incorporará uma **Camada Gratuita** rigidamente estruturada sob as seguintes premissas de barreira comercial:

1. **Autenticação Obrigatória:** O acesso às ferramentas básicas exigirá login individual e controle de credenciais.
2. **Restrição Funcional:** Limitação metodológica estrita. A camada gratuita disponibilizará apenas o mapeamento básico de autocorrelação espacial (Índice de Moran Global e Local) nativo da *Metodologia SANDRA* sobre variáveis consolidadas.
3. **Restrição de Granularidade Geográfica:** Os dados e análises da camada gratuita serão restritos à visualização em nível macro (recortes estaduais ou macrorregionais). O detalhamento em nível municipal, distrital, por setor censitário ou por unidade escolar será exclusivo dos planos corporativos pagos.
4. **Exclusão de Módulos Avançados:** As funcionalidades de Inteligência Artificial Preditiva (Machine Learning), o Sistema Prescritivo de Recomendação e o Motor de Otimização Multiobjetivo não estarão acessíveis na modalidade gratuita.

---

# 8. Produtos Tecnológicos (Ativos de Propriedade Intelectual)

* **Produto 1 — Plataforma GeoEduAI:** Aplicação Web (SaaS) com dashboards gerenciais e relatórios analíticos interativos georreferenciados para tomadores de decisão.
* **Produto 2 — Motor Analítico SANDRA-Edu:** Engine algorítmica proprietária empacotada em módulos de alta performance para extração e isolamento de fatores territoriais críticos.
* **Produto 3 — Motor Prescritivo e Recomendador:** Núcleo de regras e lógica de recomendação de intervenções públicas integradas com o território.
* **Produto 4 — API de Inteligência Territorial Educacional:** Microsserviços e endpoints REST para integração e interoperabilidade de dados com sistemas corporativos legados do governo.
* **Produto 5 — Biblioteca de Otimização Multiobjetivo Educacional:** Conjunto de scripts e heurísticas computacionais otimizados para alocação de recursos orçamentários sob restrições de governança pública.

---

# 9. Formação de Recursos Humanos (PD&I)

O projeto atuará de forma direta na qualificação de pessoal técnico e acadêmico como contrapartida obrigatória do ecossistema de fomento:

* **Pós-Graduação Stricse Sensu:** Financiamento de bolsas e taxas escolares para **1 projeto de Doutorado** e **2 projetos de Mestrado** (Acadêmico ou Profissional) vinculados a ICTs parceiras.
* **Graduação:** Concessão de Bolsas de Iniciação Científica (IC) para estudantes das áreas de Ciência da Computação, Engenharia de Software, Estatística e Geografia Quantitativa.
* **Capacitação Corporativa:** Desenvolvimento de trilhas de treinamento técnico focadas em *Data Literacy*, inteligência espacial e gestão pública baseada em evidências para os desenvolvedores da plataforma e servidores dos órgãos públicos participantes dos pilotos.

---

# 10. Cronograma de Execução Físico-Financeira (36 Meses)

| Atividade / Linha de Desenvolvimento | M1-M6 | M7-M12 | M13-M18 | M19-M24 | M25-M30 | M31-M36 |
| --- | --- | --- | --- | --- | --- | --- |
| Revisão bibliográfica, modelagem teórica e especificação técnica da plataforma | **X** |  |  |  |  |  |
| Engenharia de dados, pipelines ETL e estruturação do Data Lake Educacional | **X** | **X** |  |  |  |  |
| Desenvolvimento, teste e acoplamento do Motor Analítico SANDRA-Edu |  | **X** | **X** |  |  |  |
| Modelagem, treinamento e validação dos algoritmos de IA Preditiva |  |  | **X** | **X** |  |  |
| Implementação das rotinas de Estatística Espacial e visualização SIG |  |  | **X** | **X** |  |  |
| Desenvolvimento do Motor Prescritivo e dos algoritmos de Otimização |  |  |  | **X** | **X** |  |
| Implantação de Projetos-Piloto em Secretarias parceiras e Validação Real |  |  |  |  | **X** | **X** |
| Transferência Tecnológica, registro de patentes/softwares e relatórios finais |  |  |  |  |  | **X** |

---

# 11. Enquadramento Técnico-Legal na Lei de Informática

O projeto proposto possui total aderência aos requisitos regulatórios e de conformidade estabelecidos pela **Lei nº 8.248/1991 (Lei de Informática)** para o aporte de recursos de contrapartida de PD&I obrigatórios por parte de empresas beneficiárias de incentivos fiscais do setor de TIC, sustentando-se nos seguintes pilares fundamentais:

1. **Pesquisa Aplicada e Inovação Tecnológica:** O escopo do projeto foca na transição de uma metodologia científica acadêmica (Metodologia SANDRA) para um produto comercial de alta tecnologia em escala de mercado nacional.
2. **Desenvolvimento de Software Inovador com Tecnologias de Ponta:** O projeto centra-se no desenvolvimento de algoritmos complexos de Inteligência Artificial, Aprendizado de Máquina, Otimização de Sistemas e Análise de Grafos/Espacial, atendendo à priorização setorial de fomento de software nacional inteligente.
3. **Cooperação Estratégica com ICTs:** A estrutura de governança do projeto pressupõe a execução de atividades em parceria estreita com universidades de excelência credenciadas junto ao Comitê de Área de Tecnologia da Informação (CATI).
4. **Geração de Propriedade Intelectual Nacional:** Criação de ativos computacionais tangíveis que serão formalmente registrados junto ao Instituto Nacional da Propriedade Industrial (INPI), expandindo o portfólio de patentes e registros de software do país.
5. **Formação de Capital Humano Avançado:** Garantia de investimento real na formação acadêmica de alto nível (Doutorado e Mestrado) e inserção de jovens profissionais (Iniciação Científica) no ecossistema de desenvolvimento de TIC do mercado brasileiro.

```

```
