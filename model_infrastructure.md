# Model and Infrastructure
AWS Bedrock allows users to build and scale generative AI applications by providing access to foundation models (FMs) from various AI companies

AWS Bedrock gives you managed access to multiple Foundation Models (FMs) through a single API—no model hosting, no infra wrangling.

It also provides an ability to swap models in and out without rewriting code, 

### Model selection decision tree

|Purpose|Select Model|Why|Alternatives|
|---|---|---|---|
|Need reasoning|Claude|Choose Claude when you need the strongest reasoning, analysis, and long‑context understanding.<br>Claude models consistently outperform others in structured reasoning, multi‑step logic, and safe enterprise‑grade outputs.|Cohere Command — good for structured business logic and deterministic outputs.<br> Llama — strong reasoning if you need open‑weight control or on‑prem deployment.<br> Titan Text — acceptable for simpler reasoning tasks with lower cost.
|Need embeddings|Titan|Choose Titan Embeddings when you need high‑quality semantic vectors for search, RAG, clustering, or recommendations.<br>itan Embeddings are optimized for AWS RAG pipelines, vector search, and semantic similarity.|•  Cohere Embed — strong multilingual embeddings.<br> Llama Embeddings — good if you want open‑weight embeddings.<br>OpenSearch k‑NN — not a model, but a vector store that pairs well with Titan.
•  Need open‑weight → Llama
•  Need enterprise text → Cohere
•  Need images → Stability
</pre>
