# LLM-summariser

This notebook explores the idea of using LLMs for document summarisation. Although the initial proof of concept involves long podcast/interview transcripts the project could be extended to other documents (i.e. news articles, research papers, applications etc.)

---

## Description

Document summaries should be detailed and entity-centric without being overly dense and hard to follow. LLMs, especially those with larger context windows, paired with specific prompt engineering, can provide effective summaries comparable to human written summaries (but naturally with better efficiency).
Summary tools built off the foundation of such work could save hours, extracting insights from information rich text.

### Project:

1. **Web Scraping:** Fetching interview transcipts for summarisation - https://healthliteracy.com/podcast-transcripts/
2. **Data Cleaning:** Processing raw transcripts to extract and organise the inteviews into unique podcasts and speakers.
3. **Summarization with LLMs:** Utilizes state-of-the-art LLMs like GPT-4 or alternative open-source LLMs for concise summaries.
- Packages such as exllama(v2) utilised to allow the use of quantised LLMs
- Flexibility between paid API calls (like GPT-4) and open-source LLMs compatible with consumer-grade GPUs
4. **Prompt Engineering:** Leverage sophisticated prompt engineering for optimal results, including Chain of Density Prompting - https://arxiv.org/abs/2309.04269
