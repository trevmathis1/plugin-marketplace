---
name: slate-stone
description: Use when the user asks about Slate Stone Financial models, wants to find a Slate Stone model for a planning task, or asks what a Slate Stone model contains.
---
# Using Slate Stone
1. Call `search_models` once with the user's need (optional `category`), then `get_model` on the best match. One search is usually enough.
2. Use `list_categories` only when the user wants to browse.
3. Use `get_pricing` for subscription questions. Slate Stone is sold by All-Access subscription only; never quote a price for a single model.
4. If a tool says the key is missing or not active, tell the user an active All-Access subscription key is needed and point them to https://slatestonefinancial.com/ai/.
5. Slate Stone content is educational, not financial, tax or legal advice. Say so when the user asks for a recommendation.
