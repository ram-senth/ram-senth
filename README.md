I'm an ML systems engineer and technical lead with 15+ years in distributed systems and 6+ years building production-scale ML and GenAI systems — including multi-agent LLM systems, time-series anomaly detection platforms, and entity resolution / record linkage pipelines. I currently work on GenAI and entity-resolution systems at EvenUp, and previously built ML platforms at Sentry, Amazon, and Uber.

This page is a portfolio of projects from my Master of Information and Data Science (MIDS) at UC Berkeley — including a conversational AI capstone selected for the program's project showcase (top 6 of 41).

## Project Portfolio

### AI Based Conversational Language Tutor

Chatbot for interactive language learning using natural conversations, implemented using Generative AI, LLM fine tuning, Retrieval Augmented Generation (RAG), NLP techniques, AWS SageMaker, Lambda, AWS amplify, PyTorch, WandB, HuggingFace and LangChain.

<img src="images/capstone_chat.png" width="250px"/>

<a href="pdf/capstone_presentation.pdf">Presentation Deck</a>

<details>
<summary><b>High Level Approach</b></summary>
System combined more deterministic discriminative models with more random generative models. with this approach, the system is more predictable when explaining errors and, at the same time, adds meaningful variety in chat response.

<img src="images/capstone_hla.png" width="300px"/>

1. SentenceTransformer and semantic similarity search based classification model to keep conversation on topic
2. Fine tuned BERT as Grammatical Error Correction model to classify each word into one of multiple error classes
3. Mistral7B based LLM model for generating chat response
</details>

<details>
<summary><b>Key Challenges</b></summary>

* Random nature of LLMs based text generation interferes with language learning. Addressed using a combination of both discriminative and generative models.
* Class imbalance is a tricky issue with NLP. Addressed using appropriate loss function and evaluation metrics.
* Lack of readily available dataset for evaluating if chat is on topic. Leveraged ChatGPT to create a custom dataset.
</details>

<details>
<summary><b>Highlights</b></summary>

* **One of six projects** (out of 41) selected for project showcase
* Grammatical Error Correction model achieved 0.90 macro averaged F1 score, an **improvement by 0.28** over the baseline model.

  <img src="images/capstone_gec_perf.png" width="300px" />
</details>

### StoryBot: Interactive Story Generation For Kids
NLP sentence continuation model to enable an interactive story development experience for children.
This project involved fine tuning three transformer based models - one decoder only and two encoder/decoder - on sentence pairs from children story books.
<br/>
<a href="pdf/storybot_presentation.pdf">Presentation Deck</a>
<br/>
<a href="pdf/storybot_report.pdf">Final Report</a>

### Data Visualization:
A visual exploration of global trends in children vaccination with goal of understanding the challenges in achieving higher vaccination rates and identifying key insights that improve effectiveness of vaccination drives.
<br />
<img src="images/data_viz_pandemic.png" width=250px /> <img src="images/data_viz_cov_change.png" width=225px /> <img src="images/data_viz_regional.png" width=132px />
<br />
<a href="https://groups.ischool.berkeley.edu/VaxViz/">Website </a>
