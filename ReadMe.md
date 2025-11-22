MarketPulse: Competitive App Intelligence Pipeline
📋 Overview
MarketPulse is an NLP-driven competitive intelligence tool designed to benchmark mobile applications against their direct competitors.

In crowded app marketplaces, understanding your own user feedback is not enough—you need to know what users hate about your rivals. This project scrapes, analyzes, and compares user sentiment across multiple target applications to uncover:

Feature Gaps: What are competitors doing better?

Market Opportunities: What are users complaining about in rival apps that we can solve?

Sentiment Benchmarking: How does our "Bug Rate" compare to the industry standard?

🏗️ Architecture & Methodology
The pipeline utilizes a comparative architecture, processing multiple data streams simultaneously to generate side-by-side analytics.

1. Multi-Source Ingestion
Input: A dictionary of Target App vs. Competitor Apps (List of PlayStore IDs).

Process: Dynamic scraping of review metadata across the specified cohort to build a comparative dataset.

2. NLP Analysis Engine (Hybrid Approach)
Sentiment Scoring: Uses Hugging Face Transformers (distilbert) to assign granular sentiment scores (-1.0 to +1.0) to every review.

Topic Modeling: (Planned) Clustering reviews to detect dominant topics (e.g., "Login," "Payment," "UI") across the entire market segment.

3. Strategic Reasoning (LLM Layer) [In-Progress]
Contextual Categorization: An LLM (Llama/GPT) classifies negative reviews into strategic buckets:

🚨 Critical Failures: (Crash, Data Loss)

📉 Churn Drivers: (Ads too frequent, Subscription cost)

💡 Missing Features: (Features present in Competitor X but missing here)

🛠️ Tech Stack
Language: Python

ML Frameworks: PyTorch, Hugging Face transformers

Data Processing: Pandas (for pivot tables and aggregations)

Visualization: Matplotlib/Seaborn (for comparative heatmaps)

🚀 Roadmap
[x] Phase 1: Build Multi-App Scraper (Target vs. Competitors).

[x] Phase 2: Implement Comparative Sentiment Analysis (Transformer-based).

[ ] Phase 3 (Current): Integrate LLM for "Gap Analysis"—automatically identifying features requested in our app that exist in competitor apps.

[ ] Phase 4: Develop a Streamlit Dashboard for real-time "Head-to-Head" visualization.

[ ] Phase 5 (Juspay Alignment): Implement RAG (Retrieval Augmented Generation) to allow users to "Chat with the Reviews" (e.g., "Compare the login issues between App A and App B").

💻 Installation & Usage:

# Clone the repository
git clone https://github.com/yourusername/market-pulse.git

# Install dependencies
pip install -r requirements.txt
