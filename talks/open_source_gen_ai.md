# Open Source and Gen AI

James Healy

[Harnessing Open Source Solutions in the Generative AI Landscape](https://www.socallinuxexpo.org/scale/22x/presentations/harnessing-open-source-solutions-generative-ai-landscape)

- We often rely on companies for gen AI models instead of hosting our own
- llama-factory really nice python package, has a good cli
- vLLM engineering still using GPUs
- Why? Lots of benefits for DIY: lower latency, don't have to pay for each request on top of your own hardware, better fine tuning, can have smaller models for smaller tasks
- llama-factory good things: cli, yaml file configs
- vllm python package
- use OpenAI package with everything. Just swap out OpenAI for localhost
- can use pydantic schemas to get out line items that match schema
- Can set up RLHF yourself too

Reasoning models
- o1 and o1-mini the first ones released, but didn't show reasoning chain
- Can use Qwen models to see reasoning chain
- Remember custom models have boot up time!

Reasoning demos
- 9.8 vs 9.11 comparison demo
- comparing prices
- analyze Pokemon data set

RAG
- Fun with vector databases
- Uses reranking model (reranks results)
- Needs to handle enough tokens — set via config
- Now try with more load! Send everything in parallel, through one local GPU (it works!)

Question notes
- Unsloth quantization models
- How to handle structured data
- How it works with metaflow
- What about bigger models? Some models are smaller and can also use quantization
