# 📋 Instruções para Extração de Informações das Transcrições

## 🎯 Objetivo

Este guia detalha como extrair informações corretamente das transcrições de reuniões comerciais para criar um HTML completo com síntese da proposta comercial.

---

## 📚 Estrutura de Extração

### 1. **IDENTIFICAÇÃO DO CONTEXTO**

#### 1.1 Informações Básicas da Empresa Cliente

- **Nome da empresa**: Procurar menções explícitas
- **Número de colaboradores**: Buscar números mencionados (ex: "66 colaboradores")
- **Setores envolvidos**: Identificar departamentos mencionados (RH, DP, Gestão de Pessoas)
- **Pessoas-chave**: Nomes dos participantes e seus cargos

**Exemplo de extração:**

```
Empresa: Bidweb
Colaboradores: 66
Participantes: 
- Thuanne (Coordenadora RH)
- Sineide (Departamento Pessoal)
- Lucila (Gestão de Pessoas)
- Victor (Factorial - Vendedor)
```

---

### 2. **DORES E PROBLEMAS IDENTIFICADOS**

#### 2.1 Como Identificar Dores

Procure por:

- Frases que começam com "Nós temos problema com..."
- Menções de sistemas atuais que não funcionam bem
- Queixas sobre processos manuais
- Dificuldades mencionadas explicitamente

#### 2.2 Estrutura de Extração de Dores

Para cada dor identificada, extraia:

```
DOR #X: [Título da Dor]
- Contexto: [O que foi dito sobre o problema]
- Sistema atual: [Qual plataforma está sendo usada]
- Impacto: [Por que isso é um problema]
- Citações relevantes: [Trechos exatos da transcrição]
```

**Exemplo prático:**

```
DOR #1: Múltiplas Plataformas Desconectadas
- Contexto: Uso de três plataformas diferentes (Recrutei, Feedz, Icarus)
- Sistema atual: Recrutei (recrutamento), Feedz (desempenho), Icarus (ponto)
- Impacto: Falta de integração, necessidade de exportar/importar dados manualmente
- Citação: "A gente utiliza a Recrutei para fazer recrutamento de seleção. 
           E já usei a Solides no passado. que a Solidis é uma plataforma que 
           oferece aí uma união desses recursos"
```

---

### 3. **SOLUÇÕES PROPOSTAS**

#### 3.1 Como Identificar Soluções

Procure por:

- Frases que começam com "A gente resolve isso..."
- "A Factorial faz..."
- "Vocês vão ter..."
- Demonstrações de funcionalidades

#### 3.2 Estrutura de Extração de Soluções

Para cada solução, extraia:

```
SOLUÇÃO PARA DOR #X: [Título da Solução]
- Funcionalidade: [O que a solução faz]
- Benefício: [Por que isso resolve o problema]
- Diferencial: [O que torna isso especial]
- Citações relevantes: [Trechos exatos]
```

**Exemplo prático:**

```
SOLUÇÃO PARA DOR #1: Sistema Único Integrado
- Funcionalidade: Recrutamento, admissão, desempenho, ponto, férias e documentos em uma plataforma
- Benefício: Elimina necessidade de trocar sistemas e exportar/importar dados
- Diferencial: Fluxo completo do recrutamento à admissão digital sem troca de sistemas
- Citação: "Então vamos fazer o seguinte, eu normalmente gosto de fazer uma trilha que é, 
           desde a parte que eu não tenho nenhum candidato, eu tenho que encontrar essa 
           pessoa no recrutamento"
```

---

### 4. **CUSTOS E INVESTIMENTO**

#### 4.1 Informações Financeiras a Extrair

- **Custo mensal total**: Valor mencionado explicitamente
- **Custo por colaborador**: Valor unitário
- **Descontos especiais**: Black Friday, promoções
- **Implementação**: Custo inicial (se houver)
- **Modelo de cobrança**: Por vida, fixo, variável

#### 4.2 Estrutura de Extração de Custos

```
INVESTIMENTO:
- Custo mensal total: R$ [valor]
- Custo por colaborador: R$ [valor] / mês
- Número de colaboradores: [número]
- Desconto aplicado: [%] (Black Friday, etc.)
- Implementação: R$ [valor] (ou gratuita)
- Economia mensal: R$ [valor]
- Total com desconto: R$ [valor]
```

**Exemplo prático:**

```
INVESTIMENTO:
- Custo mensal total: R$ 2.217,50 (sem desconto)
- Custo por colaborador: R$ 23,75 / mês
- Número de colaboradores: 66
- Desconto aplicado: 25% (Black Friday)
- Implementação: R$ 0 (era R$ 3.500)
- Economia mensal: R$ 553,50
- Total com desconto: R$ 1.664 / mês
```

**Citação relevante:**

```
"Ponto, férias, denúncias, desempenho, pesquisa, gestão de treinamentos. 
Dá R$28,70 para o colaborador mensal. Multiplica R$28,70 pelo R$60. 
Dá mais ou menos R$1.700."
```

---

### 5. **MÓDULOS E FUNCIONALIDADES**

#### 5.1 Como Identificar Módulos

Procure por:

- Listas de funcionalidades mencionadas
- Demonstrações de telas/sistemas
- Comparações com sistemas atuais
- Recursos específicos destacados

#### 5.2 Estrutura de Extração de Módulos

Para cada módulo, extraia:

```
MÓDULO: [Nome do Módulo]
- Substitui: [Sistema atual que será substituído]
- Funcionalidades principais:
  • [Funcionalidade 1]
  • [Funcionalidade 2]
  • [Funcionalidade 3]
- Diferenciais: [O que torna especial]
- Citações: [Trechos relevantes]
```

**Exemplo prático:**

```
MÓDULO: Recrutamento e Seleção
- Substitui: Recrutei
- Funcionalidades principais:
  • Integração com 25+ portais (LinkedIn, InfoJobs, Indeed)
  • Página de carreiras personalizável
  • Triagem por IA com match automático
  • Teste DISC integrado
  • Fluxo kanban personalizável
  • Carta oferta digital com assinatura eletrônica
- Diferenciais: Não precisa cadastro prévio para candidatos, IA própria
- Citação: "Quando eu clico para me candidatar, eu vejo as informações, 
           a descrição dessa vaga, beleza, tudo bem, mas eu não tenho aquela 
           parte chata... você vai se candidatar na Gup, ou na Sólides, você 
           tem que criar um login na Sólides para depois fazer o envio do formulário? 
           Esquece isso, não precisa."
```

---

### 6. **CRONOGRAMA E PRÓXIMOS PASSOS**

#### 6.1 Informações Temporais a Extrair

- **Prazo para fechamento**: Datas mencionadas
- **Cronograma de implementação**: Etapas e prazos
- **Condições especiais**: Validade de descontos
- **Próximos passos**: O que precisa acontecer

#### 6.2 Estrutura de Extração de Cronograma

```
CRONOGRAMA:
- Prazo para fechamento: [data] (para aproveitar desconto)
- Implementação: [prazo estimado]
- Go-live: [data estimada]
- Etapas:
  1. [Etapa 1] - [prazo]
  2. [Etapa 2] - [prazo]
  3. [Etapa 3] - [prazo]

PRÓXIMOS PASSOS:
- [Ação 1]
- [Ação 2]
- [Ação 3]
```

**Exemplo prático:**

```
CRONOGRAMA:
- Prazo para fechamento: Até 21 de Novembro 2025 (Black Friday)
- Implementação: Início em Dezembro 2025
- Go-live: Janeiro 2026
- Etapas:
  1. Fechamento do contrato - Até 21/11/2025
  2. Reunião de handover - Até 25/11/2025
  3. 1ª Reunião de implementação - Até 05/12/2025
  4. Go-live completo - Janeiro 2026
  5. Desativação de sistemas antigos - Fevereiro 2026

PRÓXIMOS PASSOS:
- Reunião com diretor financeiro
- Envio de material de segurança para compliance
- Teste de 15 dias do módulo de ponto
```

---

### 7. **DETALHES TÉCNICOS E ESPECÍFICOS**

#### 7.1 Informações Técnicas Importantes

- **Integrações**: Sistemas que se conectam
- **API**: Disponibilidade e uso
- **Segurança**: Certificações mencionadas
- **Importação de dados**: Como fazer migração
- **Personalizações**: O que pode ser customizado

#### 7.2 Estrutura de Extração Técnica

```
DETALHES TÉCNICOS:
- Integrações: [lista de integrações]
- API: [disponibilidade e uso]
- Segurança: [certificações]
- Importação: [como fazer]
- Personalização: [o que pode ser customizado]
```

---

## 🔍 PROCESSO DE EXTRAÇÃO PASSO A PASSO

### Passo 1: Leitura Inicial

1. Leia toda a transcrição uma vez para entender o contexto geral
2. Identifique os participantes e seus papéis
3. Identifique o objetivo da reunião

### Passo 2: Extração por Categorias

1. **Primeira passada**: Extraia informações básicas (empresa, pessoas, números)
2. **Segunda passada**: Identifique todas as dores mencionadas
3. **Terceira passada**: Identifique todas as soluções propostas
4. **Quarta passada**: Extraia informações financeiras
5. **Quinta passada**: Liste todos os módulos e funcionalidades
6. **Sexta passada**: Extraia cronograma e próximos passos

### Passo 3: Validação e Organização

1. Verifique se cada dor tem uma solução correspondente
2. Confirme números e valores mencionados
3. Organize as informações em ordem lógica
4. Identifique citações-chave para destacar

### Passo 4: Estruturação para HTML

1. Organize as informações no formato que será usado no HTML
2. Identifique seções principais:
   - Resumo Executivo
   - Dores e Soluções
   - Custos
   - Escopo e Cronograma
   - Próximos Passos
3. Prepare dados para gráficos (se aplicável)
4. Identifique destaques visuais importantes

---

## 📝 CHECKLIST DE EXTRAÇÃO

Use este checklist para garantir que todas as informações foram extraídas:

### Informações Básicas

- [ ] Nome da empresa cliente
- [ ] Número de colaboradores
- [ ] Participantes da reunião e cargos
- [ ] Data da reunião (se mencionada)

### Dores Identificadas

- [ ] Lista completa de problemas mencionados
- [ ] Sistema atual usado para cada dor
- [ ] Impacto de cada problema
- [ ] Citações relevantes para cada dor

### Soluções Propostas

- [ ] Solução para cada dor identificada
- [ ] Funcionalidades específicas mencionadas
- [ ] Diferenciais destacados
- [ ] Comparações com sistemas atuais

### Informações Financeiras

- [ ] Custo mensal total
- [ ] Custo por colaborador
- [ ] Descontos aplicados
- [ ] Custo de implementação
- [ ] Economia gerada
- [ ] Modelo de cobrança

### Módulos e Funcionalidades

- [ ] Lista completa de módulos incluídos
- [ ] Funcionalidades de cada módulo
- [ ] Sistemas que serão substituídos
- [ ] Diferenciais técnicos

### Cronograma

- [ ] Prazo para fechamento
- [ ] Etapas de implementação
- [ ] Datas importantes
- [ ] Próximos passos definidos

### Detalhes Técnicos

- [ ] Integrações disponíveis
- [ ] API e customizações
- [ ] Segurança e compliance
- [ ] Processo de migração

---

## 💡 DICAS IMPORTANTES

### 1. Atenção aos Números

- Sempre confirme valores mencionados
- Verifique se há cálculos implícitos (ex: custo total = custo unitário × quantidade)
- Identifique se valores são com ou sem desconto

### 2. Contexto é Fundamental

- Não extraia informações isoladas
- Entenda o contexto completo antes de extrair
- Relacione dores com soluções

### 3. Citações Diretas

- Use citações diretas quando possível
- Isso adiciona credibilidade ao HTML
- Destaque frases impactantes do vendedor

### 4. Organização Lógica

- Organize informações em ordem de importância
- Agrupe informações relacionadas
- Crie uma narrativa coerente

### 5. Validação Cruzada

- Se uma informação aparece múltiplas vezes, confirme
- Verifique consistência entre diferentes partes da transcrição
- Identifique contradições (se houver)

---

## 🎨 PREPARAÇÃO PARA HTML

Após a extração, organize as informações neste formato:

```markdown
# PROPOSTA COMERCIAL - [NOME DA EMPRESA]

## 1. RESUMO EXECUTIVO
- Investimento mensal: R$ [valor]
- Custo por colaborador: R$ [valor]
- Economia: [%] ou R$ [valor]
- Número de colaboradores: [número]

## 2. DORES E SOLUÇÕES
### Dor 1: [Título]
- Problema: [descrição]
- Solução: [descrição]
- Diferencial: [destaque]

### Dor 2: [Título]
...

## 3. CUSTOS
- Estrutura detalhada
- Descontos aplicados
- Comparação com custos atuais

## 4. MÓDULOS INCLUÍDOS
- Lista completa
- Funcionalidades principais
- Sistemas substituídos

## 5. CRONOGRAMA
- Etapas e prazos
- Próximos passos
```

---

## ✅ EXEMPLO COMPLETO DE EXTRAÇÃO

Veja o arquivo `index.html` como exemplo de como as informações extraídas foram estruturadas em um HTML completo e profissional.

---

## 📞 SUPORTE

Se tiver dúvidas durante a extração:

1. Releia a seção específica desta instrução
2. Consulte o exemplo no `index.html`
3. Verifique se todas as informações do checklist foram extraídas

---

**Última atualização**: Baseado na análise das transcrições do projeto Bidweb/Factorial
