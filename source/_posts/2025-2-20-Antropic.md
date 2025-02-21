---
title: Antropic - The Best LLM Provider?
date: 2025-02-20 21:44:10
tags:
 - Personal Growth
 - Technology
---


## Message from the author
It's my second blog post! After busy day work @ Databricks, I don't want to do any more coding😠. So instead... begin reading some Anthropic's paper, because why not lol. Found lots of blog/papers that are really interesting.

<figure class="post-figure">
    <img src="/img/2025-2-20Antropic.png"  class="post-image" width="500" height="500">
    <figcaption>Anthropic's focusing on safety and alignment. It's very novel and interesting.</figcaption>
</figure>

## What is Antropic?

Some people might not even know this company. Simple words: It's competitor of OpenAI. It builds Claude which is one of the most popular LLM, especially for its ability in helping with coding. Although both focusing on LLM, they are very different.


## Why I like it?

A lot of LLM companies nowadays are grinding for the best performance. All of the LLM are beating eac other in terms of accuracy in some benchmarks. I feel like this is a waste of resources. Novelty needs to be valued here. They should focus on new things to better help people. As customer, I don't care about perfmrance being 1% better in math or computer science. I just want either cheap models or models that are truely different. When GPT3 first came out, it's not the best. But it's novel and useful. However, now it's just a standard. New extensions need to be made.

## What is Anthropic doing differently?

Anthropic is focusing on safety and alignment. As mentioned in their [research principles](https://www.anthropic.com/research), they want to build a safe, scable, and systamatic AI. 

A lot of interesting thigns they did is..
### [Model Context Protocol(MCP)](https://www.anthropic.com/news/model-context-protocol)

Model Context Protocol is truely one of it's kind. As we entered the era of agentic workflow. Different LLM are using different ways to call API, access data, and more. Nothing is standardized or unified. 

MCP breaks this barrier. It's provides a unified way to call API, access person data, soon even authentication. There already exists more than 30 MCP servers within their [open source github repo](https://github.com/modelcontextprotocol/servers). 

Imagine you are connected github MCP server. You simply have to enter text in your prompt, to create repo, add files, commit, and more. It abstracts all the complexity of API calls and data storage. Further more it's secure and private.

The drawback of this is that it's only supported by Anthropic's models. However, it's still a great step towards standardization. If other LLM providers want to support MCP, they are conceding to Anthropic's standard(so I bet they won't do it😂).


### [Constitutional Classifiers](https://www.anthropic.com/news/constitutional-classifiers)

Anthropic is also focusing on heavily on safety. They are building a safety model that can detect/filter harmful content, which I belive is important when we want to productionize LLM as a well-rounded assistant. 

It provides 3 layers of safety:
1. **Input Classifier**: Detect harmful content when tokens are inputted. Some dangeorou words or concepts will be  automatically blocked even before the model sees the input.
2. **LLM Model**: The large language model is trained with safety metrics. It is heavily prompted and pretrained to not output harmful content. It will refuse to answer questions that are harmful.
3. **Output Classifier**:Output classifier will be the last line of defense. It will detect harmful content in the output. If it's detected, certains parts of the output will be masked.

They've launced a challenge for the community to improve their safety model. Anyone that can breaks through all their defenses will be awarded $20000, but I don't think anyone has succeeded yet.

However, this model is not perfect. It may be overblocking certin things. A kid asking about chemistry experiments and safety shouldn't be blocked. The line of what is harmful is still blurry. However this is good advancement that I believe all LLM providers should focus on IMO.


I rather want a safer model than a better model. Imagine deploying a project that utlize LLM. But there are malicous users hacking into the model and displaying harmful content. This is a big issue. This will completely damanage your product's reputation!

That's why I out of all the LLM providers, as of moment I like Anthropic the most. Hopefully they can keep up the good work!




