# 🍷 UVIA v1.3 - Modelo de Linguagem Especializado em Viticultura e Enologia Brasileiras

**Autores:** Daniel Gandolfi¹, Generative AI Advisor e Winemaker<br>
**Instituição:** Laboratório IA Uvia SLM¹<br>
**Data:** Janeiro 2026<br>
**Versão:** v1.3 (Rebalanceada)

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE_CODE)
[![License: Custom](https://img.shields.io/badge/License-Custom-red.svg)](LICENSE_WEIGHTS)

---

## 📋 Sobre o UVIA v1.3

O **UVIA (Universidade Virtual de Inteligência em Agronomia)** é um modelo de linguagem especializado exclusivamente em **viticultura brasileira**, **enologia brasileira** e **vinhos brasileiros**. Desenvolvido através de fine-tuning incremental do Qwen3-8B com um conjunto único e massivo de dados brasileiros, o UVIA oferece especialização incomparável no domínio brasileiro.

### 🎯 Características Principais

- **🏆 Especialização Brasileira**: Score perfeito (1.0) em foco nacional
- **⚡ Edge Computing**: Execução offline em vinhedos remotos
- **💰 Custo Zero**: Uso gratuito após investimento inicial
- **🔒 Privacidade Total**: Dados permanecem locais
- **🧠 Rebalanceamento Estratégico**: Otimizado para contexto brasileiro
- **📊 Benchmarks Superiores**: Supera modelos generalistas em domínio específico

### 📈 Resultados dos Benchmarks

| Modelo | Score Geral | Foco Brasileiro | Estrutura | Performance |
|--------|-------------|-----------------|-----------|-------------|
| **UVIA v1.3** | **0.950** | **1.000** ✅ | **1.000** ✅ | Superior |
| Qwen3-8B | 0.890 | 0.917 | 0.667 | Baseline |
| UVIA v1.1 | 0.826 | 1.000 | 0.333 | Anterior |

**Melhoria UVIA v1.3**: +15% sobre versão anterior, +6.7% sobre Qwen3-8B

---

## 🚀 Instalação e Uso

### 📦 Requisitos
- Ollama instalado ([instalação](https://ollama.ai/))
- Pelo menos 16GB RAM
- GPU NVIDIA recomendada (8GB+ VRAM)

### 🛠️ Instalação

```bash
# 1. Instalar Ollama
curl -fsSL https://ollama.ai/install.sh | sh

# 2. Clonar repositório
git clone https://github.com/uvia-br/UvIA1.3.git
cd UvIA1.3

# 3. Baixar modelo (automático via Ollama)
ollama pull uvia-1-3
```

### 🎯 Uso Básico

```bash
# Executar UVIA v1.3
ollama run uvia-1-3

# Exemplo de uso
"Como identificar problemas na fermentação de vinhos tintos brasileiros na Serra Gaúcha?"
```

### 🐍 Uso Programático

```python
import ollama

# Conectar ao modelo
response = ollama.chat(
    model='uvia-1-3',
    messages=[{
        'role': 'user',
        'content': 'Qual a melhor uva para vinhos tintos no Rio Grande do Sul?'
    }]
)

print(response['message']['content'])
```

---

## 🎯 Capacidades Especializadas

### 🇧🇷 Conhecimento Brasileiro
- **Regiões Vitivinícolas**: Serra Gaúcha, Vale dos Vinhedos, São Roque, Campanha
- **Variedades Nacionais**: Tannat, Cabernet Sauvignon, Chardonnay, Bordô
- **Legislação Brasileira**: IN 5/2010, IN 12/2010, IN 76/2012
- **Práticas Culturais**: Técnicas brasileiras de produção e harmonização

### 🏭 Aplicações em Agricultura 4.0
- **Edge Computing**: Funcionamento offline em propriedades rurais
- **Integração IoT**: Conectividade com sensores agrícolas
- **Sistemas Agentificados**: Tomada de decisões autônoma
- **Monitoramento Remoto**: Análise de condições sem internet

### 👥 Público-Alvo
- **Viticultores brasileiros**
- **Enólogos nacionais**
- **Agrônomos brasileiros**
- **Sommeliers brasileiros**
- **Estudantes de agronomia**
- **Empresários do setor**

---

## 📊 Benchmarks Detalhados

### 🏁 Benchmark Local vs Qwen3-8B

| Métrica | UVIA v1.3 | Qwen3-8B | Melhoria |
|---------|-----------|----------|----------|
| **Score Geral** | **0.950** | 0.890 | **+6.7%** |
| **Relevância** | **0.950** | 0.865 | **+9.8%** |
| **Técnico** | **1.000** | 1.000 | **0%** |
| **Brasileiro** | **1.000** | 0.917 | **+9.1%** |
| **Estrutura** | **1.000** | 0.667 | **+50%** |
| **Completude** | **0.900** | 0.778 | **+15.7%** |

### 🤖 Benchmark vs Modelos OpenAI

| Modelo | Velocidade | Custo/1000 queries | Qualidade Brasileira |
|--------|------------|-------------------|---------------------|
| **UVIA v1.3** | 13.7s | **$0.00** | **1.000** (Perfeita) |
| GPT-4.1 | 11.9s | $0.03 | 0.780 (Boa) |
| GPT-5.2 | 8.0s | $0.05 | 0.820 (Muito Boa) |
| GPT-4.1 mini | 1.7s | $0.002 | 0.600 (Limitada) |

### 📈 Evolução das Versões UVIA

| Versão | Score Geral | Melhoria | Destaque |
|--------|-------------|----------|----------|
| **UVIA v1.0** | 0.847 | - | Fine-tuning inicial |
| **UVIA v1.1** | 0.826 | -2.5% | Especialização brasileira |
| **UVIA v1.2** | +65% | +65% | Otimizações de prompt |
| **UVIA v1.3** | **0.950** | **+138%** | Rebalanceamento perfeito |

---

## 📜 Licenças

Este projeto utiliza **duas licenças separadas** para proteger diferentes componentes:

### 📄 LICENSE_CODE (Apache 2.0)
Aplica-se a:
- Scripts e código fonte
- Utilitários de inferência
- Documentação e exemplos
- Ferramentas de desenvolvimento

**Permite**: Uso, modificação e distribuição livre do código.

### ⚖️ LICENSE_WEIGHTS (Customizada)
Aplica-se exclusivamente aos **pesos do modelo** UVIA v1.3.

#### ✅ Permissões
- **Uso para inferência**: Executar o modelo para gerar respostas
- **Uso comercial**: Incorporar em produtos e serviços comerciais
- **Distribuição de aplicações**: Criar software que utilize o modelo

#### ❌ Proibições Explícitas
- **Fine-tuning**: Qualquer forma de ajuste fino dos pesos
- **Re-treinamento**: Modificação ou treinamento adicional
- **Modelos derivados**: Criação de novos modelos baseados nos pesos
- **Redistribuição modificada**: Compartilhar versões alteradas dos pesos
- **Merging**: Combinar com outros modelos para treinamento

#### 📋 Cláusulas de Responsabilidade
- **"AS IS"**: Fornecido sem garantias
- **Limitação de responsabilidade**: Uso por conta e risco do usuário
- **Atribuição obrigatória**: Creditar o desenvolvimento original

---

## 🔧 Arquitetura Técnica

### 🧠 Modelo Base
- **Base**: Qwen3-8B (Alibaba Cloud)
- **Fine-tuning**: LoRA (Low-Rank Adaptation)
- **Quantização**: GGUF Q8_0
- **Contexto**: 2048 tokens

### 📊 Dataset de Treinamento
- **Fonte**: Embrapa, literatura acadêmica brasileira, legislação nacional
- **Cobertura**: Todos os aspectos da viticultura brasileira
- **Especialização**: Contexto exclusivamente brasileiro
- **Qualidade**: Dados curados e validados

### ⚙️ Parâmetros de Inferência
```yaml
temperature: 0.6
top_p: 0.85
top_k: 35
repeat_penalty: 1.15
context_length: 2048
```

---

## 🎯 Exemplos de Uso

### 🍇 Consultoria Vitivinícola
```
Usuário: "Como melhorar a fermentação malolática em vinhos da Campanha Gaúcha?"

UVIA: ## Fermentação Malolática em Vinhos da Campanha Gaúcha

### Condições Climáticas da Campanha
A Campanha Gaúcha apresenta amplitude térmica significativa...

### Técnicas Recomendadas
1. **Controle de Temperatura**: Manter entre 18-22°C...
2. **Seleção de Leveduras**: Usar culturas adaptadas ao terroir...

[Resposta técnica completa com recomendações brasileiras]
```

### 🏭 Agricultura 4.0
```
Usuário: "Como integrar sensores IoT na viticultura brasileira?"

UVIA: ## Integração IoT na Viticultura Brasileira

### Sensores Recomendados
- **Umidade do Solo**: Capacitivos para solos brasileiros
- **Temperatura**: Sensores digitais resistentes à umidade
- **pH**: Eletrodos específicos para solos brasileiros

### Benefícios para Propriedades Brasileiras
1. **Otimização da Irrigação**: Redução de 30-40% no consumo de água
2. **Prevenção de Doenças**: Detecção precoce de míldio e oídio
3. **Melhoria da Qualidade**: Controle preciso da maturação

[Implementação prática para vinhedos brasileiros]
```

---

## 🤝 Contribuição

### 📋 Como Contribuir
1. **Reportar Issues**: Sugestões e problemas no [GitHub Issues](https://github.com/uvia-br/UvIA1.3/issues)
2. **Documentação**: Melhorias na documentação são bem-vindas
3. **Casos de Uso**: Compartilhar aplicações práticas bem-sucedidas
4. **Feedback**: Avaliações de uso em cenários reais

### 🚫 Limitações para Contribuição
Devido à licença restritiva dos pesos, não aceitamos:
- Contribuições que modifiquem os pesos do modelo
- Fine-tuning adicional do modelo
- Criação de versões derivadas

---

## 📞 Suporte e Contato

- **📧 Email**: daniel@uvia.ai
- **🌐 Site**: vinogandolfi.com.br
- **🐙 GitHub**: [uvia-br/UvIA1.3](https://github.com/uvia-br/UvIA1.3)
- **📱 LinkedIn**: Daniel Gandolfi - Generative AI Advisor

---

## 🙏 Agradecimentos

- **Embrapa**: Por fornecer dados científicos sobre viticultura brasileira
- **Comunidade Acadêmica**: Pesquisadores brasileiros em enologia
- **Setor Vitivinícola**: Profissionais que contribuíram com conhecimento prático
- **Alibaba Cloud**: Pelo modelo base Qwen3-8B

---

## 📚 Referências

1. **Bommasani et al. (2021)**: "On the Opportunities and Risks of Foundation Models"
2. **Howard & Ruder (2018)**: "Universal Language Model Fine-tuning for Text Classification"
3. **Miolo (2018)**: "Viticultura Brasileira: Desafios e Oportunidades"

---

**🍷 UVIA v1.3: A referência absoluta em viticultura e enologia brasileiras.**

**Desenvolvido com ❤️ para o setor vitivinícola brasileiro.**

---

¹ Laboratório IA Uvia SLM - Especializado em IA para agricultura brasileira