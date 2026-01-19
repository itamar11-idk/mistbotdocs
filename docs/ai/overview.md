# 🤖 MistAI: Experimental Assistant Overview

MistAI is an experimental integration within the MistBot ecosystem. It utilizes a Retrieval-Augmented Generation (RAG) architecture to process AOT:R-specific documentation and provide automated responses based on official game data.

### 🔍 Current Scope of Knowledge
The system is currently indexed to provide information on the following pillars of AOT:R gameplay:

* **Mechanics Verification:** Clarification on human and titan progression, including the Prestige loop (1–5), leveling requirements, and skill tree interactions.
* **Database Queries:** Access to item-specific data, such as drop rates for Titan Serums and rarity tiers for artifacts.
* **Economic Data:** Current market estimates for trading (e.g., Key/Gem values) and secondary requirements like the Prestige 3 trading tax.

### 🛡️ Beta Limitations & Disclaimer
MistAI is currently in a **Testing Phase**. Users should be aware of the following professional constraints:

* **Model Uncertainty:** As a Large Language Model (LLM) in beta, MistAI may occasionally generate "hallucinations" or factually incorrect statements. It does not replace human verification from the staff or official Trello.
* **No Predictive Strategy:** The system is designed to retrieve existing data, not to simulate or predict "best" builds. Any recommendations should be viewed as references to current community trends found in its data source, rather than definitive gameplay advice.
* **Constraint Protocol:** If the system cannot locate a direct match within the indexed data, it is programmed to state its limitations rather than fabricate a response.

### 🧪 Development Roadmap
We are actively fine-tuning the retrieval accuracy. During this period:
1. **Usage Logs:** All queries are logged to identify "knowledge gaps" where the AI provides unsatisfactory answers.
2. **Data Patching:** The underlying index is updated following major game patches (e.g., Update 4 meta shifts) to prevent the dissemination of legacy information.
3. **Feedback Loop:** Users are encouraged to report systematic errors to the development team to assist in the training process.

!!! warning "Accuracy Notice"
    MistAI is provided "as-is" during the beta period. The MistBot team is not responsible for in-game losses or trading errors resulting from AI-generated information. Always cross-reference critical data in the #help or #trading channels.
