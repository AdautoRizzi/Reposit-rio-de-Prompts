# Guia Prático: Maximizando a Produtividade com IA

## 1. Digerir documentos longos em 5 minutos
**A dor:** Relatório de 80 páginas, contrato de fornecedor ou pesquisa de mercado. Você sabe que tem informação útil ali, mas não tem duas horas para ler.

**O fluxo:** Suba o documento no **Claude** (arraste o arquivo para o chat) ou no **NotebookLM** (adicione como fonte).

### Prompts Sugeridos:

*   **Resumo executivo:**
    > "Resuma esse documento em 5 parágrafos. O primeiro parágrafo deve conter a conclusão principal. Os outros quatro devem cobrir os pontos mais relevantes para um [seu cargo/contexto]."

*   **Extração de riscos:**
    > "Liste os riscos, ressalvas ou pontos de atenção mencionados nesse documento. Inclua a página ou seção onde cada um aparece."

*   **Perguntas diretas:**
    > "Com base nesse documento, [sua pergunta específica]." 
    > *Exemplo: "Qual é a projeção de crescimento para o segmento X em 2027?" ou "Quais cláusulas desse contrato limitam nosso direito de rescisão?"*

> [!TIP]
> **Claude vs NotebookLM:** Se é um documento único para interagir, o **Claude** funciona bem. Se precisa cruzar vários documentos (ex: três relatórios de concorrentes), o **NotebookLM** é melhor pois cita a fonte exata da resposta.

---

## 2. Preparar reunião em 3 minutos
**A dor:** Reunião em 15 minutos com alguém que você não conhece bem e sem tempo para pesquisa.

**O fluxo (antes da reunião):**
1. No **Perplexity**, pesquise: `"[nome da pessoa] + [empresa]"` ou `"[nome da empresa] + [setor]"`.
2. Cole o resultado no **Claude** com este prompt:
    > "Com base nessas informações sobre [pessoa/empresa], gere 5 perguntas inteligentes que eu possa fazer na reunião. Contexto: sou [seu cargo] e o objetivo da reunião é [objetivo]."

**O fluxo (depois da reunião):**
Se você usa transcrição (Granola, Fireflies, Otter, etc.), cole o texto no **Claude**:
> "Extraia desta transcrição: 1) as decisões tomadas, 2) os action items com responsável e prazo, 3) os pontos que ficaram em aberto. Formate como um email curto que eu possa enviar aos participantes."

---

## 3. Escrever emails profissionais que soem como você
**A dor:** Emails de IA soam genéricos e excessivamente formais.

**O hack:** Ensine o seu estilo antes de pedir o texto.
1. Cole 5 emails reais seus no **Claude** com este prompt:
    > "Analise esses 5 emails e mapeie meu estilo de escrita: tom, nível de formalidade, comprimento típico, forma de abrir e fechar, uso de vírgulas e pontos. Não me dê o resumo agora — apenas guarde esse perfil para os próximos pedidos."
2. Nos próximos pedidos, adicione: *"Escreva no meu estilo de escrita que você mapeou."*

**Prompt para situações difíceis:**
> "Preciso escrever um email para [pessoa/cargo] sobre [situação]. O tom precisa ser [firme mas respeitoso / direto sem ser agressivo / empático mas com limites claros]. Contexto: [o que aconteceu]. Objetivo: [o que quero que aconteça depois desse email]."

---

## 4. Transformar dados em narrativa para stakeholders
**A dor:** Planilhas complexas que precisam ser explicadas para quem não quer ver números puros.

**O fluxo:**
1. Exporte a planilha como **CSV** e suba no **Claude**.
2. Use este prompt:
    > "Analise esses dados e escreva um resumo executivo de 3 parágrafos como se fosse para o [diretor financeiro / VP de marketing / CEO]. Sem termos técnicos. Comece pela conclusão principal, depois mostre o que sustenta essa conclusão, e termine com uma recomendação."

**Para apresentações:**
> "Converta essa análise em 5 slides. Para cada slide, escreva o título (uma frase que comunica o insight, não o tema) e 3 bullets de suporte."

> [!IMPORTANT]
> O título do slide não deve ser "Receita Q1", mas sim **"Receita Q1 cresceu 12% puxada pelo segmento enterprise"**. O título comunica, o conteúdo sustenta.

---

## 5. Pesquisa competitiva em 20 minutos
**A dor:** Briefing de concorrentes urgente.

**O fluxo:**
1. **Perplexity:** Faça buscas como `"[concorrente] + lançamentos recentes"` ou `"[seu setor] + tendências 2026"`.
2. **NotebookLM:** Suba os resultados do Perplexity + seus relatórios internos em PDF.
3. **Pergunta:** *"Com base em todas as fontes, quais movimentos dos concorrentes representam risco ou oportunidade para nós? Organize por nível de urgência."*
4. **Finalização (Claude):** *"Transforme essa análise em um briefing de uma página para o [cargo]. Tom direto. Comece pelo que exige ação imediata."*

---

## 6. Criar SOPs e documentação de processos
**A dor:** Conhecimento crítico "preso" na cabeça de poucas pessoas.

**O fluxo:**
1. Grave um áudio da pessoa explicando o processo (fala livre).
2. Transcreva o áudio (Whisper, ChatGPT ou ferramentas de transcrição).
3. Use este prompt no **Claude**:
    > "Transforme essa transcrição em um SOP (Standard Operating Procedure) estruturado. Inclua: objetivo do processo, pré-requisitos, passo a passo numerado, responsável de cada etapa, exceções comuns e como tratá-las, e critérios de sucesso. Limpe repetições e linguagem informal, mas mantenha os detalhes técnicos exatos."

---

## 7. Automatizar follow-ups e tarefas recorrentes
**A dor:** Tarefas manuais repetitivas de final de semana ou início de mês.

**O fluxo (Templates Inteligentes):**
Crie um prompt-template fixo para cada tarefa. Exemplo para vendas:
> "Escreva um email de follow-up para [nome do contato] da empresa [empresa]. Último contato: [data]. Contexto da conversa anterior: [2 linhas]. Tom: profissional e direto, sem parecer insistente. Objetivo: [agendar próxima call / obter resposta sobre proposta / reengajar contato frio]."
