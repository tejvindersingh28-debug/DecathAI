# DecathAI — Predictive Shopping Assistant

DecathAI is an AI-powered shopping assistant designed to help people discover what they may need next based on a recent purchase, shopping patterns, and available preferences.

Instead of suggesting products at random, DecathAI considers relationships between items and the context of a customer's purchase. For example, after someone buys bread, it might suggest butter, jam, cheese, or eggs. If the bread is intended for sandwiches, it can prioritize relevant sandwich ingredients.

> **Important:** Recommendations based only on a single purchase are general product suggestions—not proven predictions of an individual's next purchase. Personalization improves when authorized purchase history and preferences are available.

## ✨ Features

- **Next-purchase recommendations** — Suggests products that may logically follow a recent purchase.
- **Context-aware suggestions** — Adjusts recommendations to the user's stated goal, such as breakfast or sandwich preparation.
- **Complementary product discovery** — Identifies useful product pairings and related items.
- **Personalization-ready design** — Can use purchase history, preferences, budget, and shopping frequency when those inputs are available.
- **Repurchase reminders** — Can estimate replenishment timing when dates and quantities are provided.
- **Explainable results** — Gives a short reason for each recommendation.
- **Conversational refinement** — Lets users narrow suggestions by budget, preferences, or purpose.

## 🛒 Example

**User:** I just purchased bread. What might I need next?

**DecathAI:**
1. **Butter** — A common spread for bread.
2. **Jam** — A sweet option for toast or breakfast.
3. **Eggs** — Useful for a breakfast meal.
4. **Cheese** — A possible option for sandwiches.
5. **Milk** — A common accompaniment to breakfast.

These are illustrative suggestions. Actual recommendations should reflect the user's context and available data.

## ⚙️ How It Works

1. **Input:** Receive a recently purchased product and, optionally, purchase history, preferences, budget, or intended use.
2. **Interpretation:** Identify the product category and relevant context.
3. **Recommendation:** Generate and rank suitable complementary or likely replenishment items.
4. **Explanation:** Provide a concise reason for each suggestion and communicate uncertainty honestly.
5. **Refinement:** Update suggestions based on the user's feedback.

## 🧠 Recommendation Principles

- Prioritize relevance over the number of products suggested.
- Explain why each item is recommended.
- Clearly distinguish personalized predictions from general product associations.
- Do not claim access to purchase history unless it is supplied by the user or an authorized integration.
- Do not invent prices, stock levels, discounts, or store details.
- Respect user-provided budgets, preferences, and dietary requirements.
- Avoid encouraging unnecessary purchases; acknowledge when no additional item is needed.
- Handle personal data responsibly and use only authorized data sources.

## 🏗️ Architecture and Integrations

DecathAI is intended to support a modular recommendation workflow. Depending on the implementation, it can be extended with:

- A product catalog or product-search API
- An authorized transaction-history source
- A preference or shopping-list store
- Product association or next-purchase recommendation logic
- An LLM API for interpreting requests and explaining recommendations
- Agentverse and the Agent Chat Protocol (ACP) for agent discovery and communication

**Integration status:** Update this section to reflect the tools and integrations actually implemented in your repository. Do not describe planned integrations as already working.

## 🚀 Getting Started

The exact setup steps depend on the Agentverse-generated implementation and the files in this repository.

1. Clone this repository.
2. Review the generated project files and its dependency manifest.
3. Follow the installation and configuration instructions provided by the implementation.
4. Configure required API keys or environment variables using a local `.env` file or the platform's secrets manager.
5. Run the agent using the command specified by the project.
6. Test with a recent purchase and verify that the recommendations and explanations are sensible.

Never commit API keys, credentials, customer transaction data, or other secrets to GitHub. If you use environment variables, document their names in an `.env.example` file with placeholder values only.

## 🧪 Suggested Test Cases

| Scenario | Expected behavior |
|---|---|
| User buys bread | Suggest relevant complementary items |
| User says the bread is for sandwiches | Prioritize sandwich-related products |
| User provides a budget | Favor options consistent with that budget, without inventing prices |
| User provides purchase history | Use only the supplied or authorized history to personalize suggestions |
| No history is available | Label results as general suggestions |
| User has dietary restrictions | Avoid suggestions that conflict with stated restrictions |
| Product information is unavailable | Ask a clarifying question or explain the limitation |

## 🛡️ Privacy and Responsible Recommendations

DecathAI should use only information that the user provides or authorizes it to access. It should not imply that it can see purchases, accounts, or store inventory without an actual integration. Recommendations should be transparent, relevant, and easy to refine.

## 🗺️ Roadmap

- [ ] Complete and test the core recommendation workflow
- [ ] Configure and verify Agent Chat Protocol (ACP) support
- [ ] Verify registration and discoverability through Agentverse and ASI:One
- [ ] Add product-catalog integration
- [ ] Add optional, authorized purchase-history personalization
- [ ] Add budget-aware ranking and replenishment estimates
- [ ] Add automated tests and error-handling coverage
- [ ] Record a short end-to-end demo

## 🤝 Contributing

Contributions and suggestions are welcome. Open an issue to propose an improvement or submit a pull request with a clear description of the change.

## 📄 License

No license has been selected yet. Add a `LICENSE` file before distributing this project under an open-source license.

---

**DecathAI — From what you bought to what you may need next.**
