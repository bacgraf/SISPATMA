# 🚫 REGRA MANDATÓRIA: PROIBIÇÃO DE SCRIPTS PARA GERAÇÃO/EDIÇÃO DE IMAGENS

Esta regra é de cumprimento **obrigatório e inegociável** para o agente de IA neste projeto (**SIPATMA / TekSea**).

---

## 1. Diretriz Principal
* **NUNCA, sob nenhuma circunstância**, utilize scripts de código (Python, Pillow, PIL, OpenCV, NumPy, Canvas, PowerShell, ImageMagick ou qualquer outra ferramenta programática) para:
  - Criar imagens, mockups, banners ou slides;
  - Fazer montagens, composições, recortes ou colagens de personagens;
  - Gerar degradês, sobreposições de texto ou fusões visuais.

---

## 2. Método Exclusivo de Criação Visual & Referência Obrigatória
* Toda e qualquer criação visual (personagens, slides de campanha, mockups de uniformes e peças gráficas) deve ser executada **EXCLUSIVAMENTE através da capacidade nativa de visão computacional / geração direta de imagens da IA (`generate_image`)**.
* **Observância Obrigatória de `modelos/Uniforme/`:** É mandatório consultar e utilizar como referência estrita os arquivos de imagens e especificações (`.md`) contidos na pasta [`modelos/Uniforme/`](../../modelos/Uniforme/) e no arquivo [`FICHAS_TECNICAS_EPIS.md`](../../FICHAS_TECNICAS_EPIS.md), garantindo fidelidade total a cortes, golas, botinas dielétricas, capacete e faixas refletivas.
* A IA deve confiar em sua própria inteligência generativa e visão de design, fornecendo prompts detalhados de iluminação, enquadramento, proporção e referências visuais reais.

---

## 3. Protocolo em Caso de Esgotamento de Cota (Erro 429)
* Se a ferramenta de geração nativa de imagens atingir o limite temporário de requisições (*Rate Limit / 429 Quota Exhausted*):
  - **NÃO TENTE contornar a limitação** escrevendo scripts de manipulação de imagem.
  - **Avise o usuário imediatamente e com clareza**, informando o tempo exato restante para o restabelecimento da cota.
  - Aguarde a reinicialização da cota ou pergunte ao usuário se ele deseja avançar em tarefas textuais, documentais ou conceituais enquanto isso.

---

## 4. Reprodução Exata de Personagens em Slides e Peças Gráficas
* **Análise por Visão Computacional:** Utilizar a visão computacional para ler, analisar e extrair as feições, proporções, cabelos, biótipo e vestimentas das fotos oficiais de cada personagem antes de qualquer criação.
* **Fidelidade Visual Absoluta:** Ao construir qualquer personagem em slides de campanha (ex: `Comportamento_Seguro`) ou materiais gráficos, ele deve ser reproduzido **EXATAMENTE como se parece na imagem oficial de sua pasta e no arquivo `perfil.md`** (sem alterar traços fisionômicos, idade, etnia, cabelo ou padrão de uniforme).

---

## 5. Conferência Prévia Mandatória de Modelos, Perfis e Fichas Técnicas
* **Auditoria Cruzada Obrigatória:** Antes de gerar qualquer slide ou composição visual, o assistente **DEVE obrigatoriamente inspecionar via visão computacional e leitura textual**:
  1. **As imagens de referência oficiais dos EPIs e uniformes** em [`modelos/Uniforme/`](../../modelos/Uniforme/) e suas especificações em [`FICHAS_TECNICAS_EPIS.md`](../../FICHAS_TECNICAS_EPIS.md) (ex.: logo da TekSea no capacete é **estritamente centralizado na frente**, nunca nas laterais; uniforme de chão de fábrica possui gola alta estruturada fechada no pescoço, vista de zíper e bolsos técnicos específicos);
  2. **A imagem oficial do personagem** na sua respectiva pasta e seu arquivo `perfil.md`;
  3. **A coerência da cena com o perfil do personagem:** A função, senioridade e postura do personagem descritas no `perfil.md` devem ser respeitadas no contexto da cena da campanha (avaliando se a atitude retratada condiz com o cargo e atribuições do colaborador na fábrica).

---
*Documento de instrução comportamental ativo para o workspace SIPATMA.*

