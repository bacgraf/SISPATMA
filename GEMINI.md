# 📋 Diretrizes Gerais do Projeto — SIPATMA / TekSea

Este arquivo define as regras e restrições mandatórias de comportamento para o assistente de IA neste repositório.

---

## 🚫 1. Proibição Absoluta de Scripts para Manipulação de Imagens
* **É expressamente proibido** utilizar scripts em Python (Pillow/PIL, OpenCV, etc.), scripts de shell ou código programático para gerar, recortar, colar, compor ou manipular imagens, personagens e slides.
* Todas as criações visuais devem ser geradas **única e exclusivamente através da visão computacional e do gerador nativo de imagens da IA (`generate_image`)**.
* Em caso de indisponibilidade ou limite de cota da API de imagem, o assistente deve comunicar a situação de forma transparente ao usuário e aguardar a liberação da cota, sem nunca tentar criar soluções de contorno via código.

---

## 🎯 2. Padrão Visual e Identidade TekSea
* **Uso Obrigatório de Visão Computacional:** O assistente deve utilizar a visão computacional para analisar detalhadamente todas as imagens de referência antes de gerar qualquer elemento, garantindo a reprodução fiel e milimétrica de uniformes, EPIs e personagens.
* **Referência Obrigatória:** Para qualquer criação visual, modelagem ou descrição de uniformes e EPIs, deve-se observar e seguir com rigor absoluto os arquivos de imagens de referência e especificações técnicas (`.md`) contidos em [`modelos/Uniforme/`](modelos/Uniforme/) e [`FICHAS_TECNICAS_EPIS.md`](FICHAS_TECNICAS_EPIS.md).
* Manter fidelidade rigorosa às especificações do projeto:
  - **Uniforme Industrial de Chão de Fábrica:** Gola alta estruturada fechada no pescoço, vista de zíper, faixas refletivas prismáticas duplas (cinza/prata com bordas amarelo-limão), bolsos técnicos, calça jeans ou calça industrial reta, capacete Classe B branco e botinas dielétricas NR-10 em nobuck marrom café (conforme imagens em `modelos/Uniforme/`).
  - **Uniforme do Almoxarifado:** Camisa polo cinza de manga curta com gola e acabamento das mangas em verde TekSea, logo bordado no peito esquerdo, calça jeans e botinas industriais.
  - **Escritório:** Sem uniforme (smart casual elegante).

---

## 👥 3. Gestão e Reprodução Fiel dos Personagens nos Slides
* **Fidelidade Fisionômica e Estética Absoluta:** Ao construir qualquer personagem em slides de campanha (ex: `Comportamento_Seguro`), peças gráficas ou materiais institucionais, o personagem deve ser reproduzido **EXATAMENTE como ele se parece na imagem oficial de sua pasta e no arquivo `perfil.md` correspondente** (mesmos traços faciais, etnia, idade, cabelos, óculos, expressão, biótipo, caimento de roupas e acessórios).
* **Organização em Pastas:** Cada personagem deve ter sua própria subpasta dentro de `modelos/Personagens/`, contendo a imagem em alta resolução e sua ficha técnica completa no arquivo `perfil.md`.
* **Nomenclatura:** Personagens genéricos não possuem nomes próprios (identificados como `Personagem_Generico_X`). Os membros com nomes específicos são reservados exclusivamente para a **CIPAA**.

---

## 🔍 4. Conferência Prévia Mandatória de Modelos, Perfis e Fichas Técnicas
* **Auditoria Cruzada Obrigatória:** Antes de gerar qualquer slide ou composição visual, o assistente **DEVE obrigatoriamente inspecionar via visão computacional e leitura textual**:
  1. **As imagens de referência oficiais dos EPIs e uniformes** em [`modelos/Uniforme/`](modelos/Uniforme/) e suas especificações em [`FICHAS_TECNICAS_EPIS.md`](FICHAS_TECNICAS_EPIS.md) (ex.: logo da TekSea no capacete é **estritamente centralizado na frente**, nunca nas laterais; uniforme de chão de fábrica possui gola alta estruturada fechada no pescoço, vista de zíper e bolsos técnicos específicos);
  2. **A imagem oficial do personagem** na sua respectiva pasta e seu arquivo `perfil.md`;
  3. **A coerência da cena com o perfil do personagem:** A função, senioridade e postura do personagem descritas no `perfil.md` devem ser respeitadas no contexto da cena da campanha (avaliando se a atitude retratada condiz com o cargo e atribuições do colaborador na fábrica).

