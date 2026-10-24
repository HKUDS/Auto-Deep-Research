<a name="readme-top"></a>

<div align="center">
  <img src="./assets/logo.jpg" alt="Logo" width="200">
  <h1 align="center">Auto-Deep-Research:</br> Your Fully-Automated and Cost-Effective Personal AI Assistant </h1>
</div>





<div align="center">
  <a href="https://metachain-ai.github.io"><img src="https://img.shields.io/badge/Project-Page-blue?style=for-the-badge&color=FFE165&logo=homepage&logoColor=white" alt="Credits"></a>
  <a href="https://join.slack.com/t/metachain-workspace/shared_invite/zt-2zibtmutw-v7xOJObBf9jE2w3x7nctFQ"><img src="https://img.shields.io/badge/Slack-Join%20Us-red?logo=slack&logoColor=white&style=for-the-badge" alt="Join our Slack community"></a>
  <a href="https://discord.gg/z68KRvwB"><img src="https://img.shields.io/badge/Discord-Join%20Us-purple?logo=discord&logoColor=white&style=for-the-badge" alt="Join our Discord community"></a>
  <a href="./Communication.md"><img src="https://img.shields.io/badge/💬Feishu-Group-07c160?style=for-the-badge&logoColor=white&labelColor=1a1a2e"></a>
  <a href="./Communication.md"><img src="https://img.shields.io/badge/WeChat-Group-07c160?style=for-the-badge&logo=wechat&logoColor=white&labelColor=1a1a2e"></a>
  <br/>
  <a href="https://metachain-ai.github.io/docs"><img src="https://img.shields.io/badge/Documentation-000?logo=googledocs&logoColor=FFE165&style=for-the-badge" alt="Check out the documentation"></a>
  <a href="https://arxiv.org/abs/2502.05957"><img src="https://img.shields.io/badge/Paper%20on%20Arxiv-000?logoColor=FFE165&logo=arxiv&style=for-the-badge" alt="Paper"></a>
  <a href="https://gaia-benchmark-leaderboard.hf.space/"><img src="https://img.shields.io/badge/GAIA%20Benchmark-000?logoColor=FFE165&logo=huggingface&style=for-the-badge" alt="Evaluation Benchmark Score"></a>
  <hr>
</div>

Welcome to Auto-Deep-Research! Auto-Deep-Research is a open-source and cost-efficient alternative to OpenAI's Deep Research, based on [AutoAgent](https://github.com/HKUDS/AutoAgent) framework.

## ✨Key Features

- 🚀 **High Performance**: Delivers good performance on GAIA Benchmark.
- 🌐 **Universal LLM Support**: Seamlessly integrates with **A Wide Range** of LLMs (e.g., OpenAI, Anthropic, Deepseek, vLLM, Grok, Huggingface ...)
- 🔀 **Flexible Interaction**: Supports both **function-calling** and **non-function-calling** interaction LLMs.
- 💰 **Cost-Efficient**: Open-source alternative to Deep Research's $200/month subscription with your own pay-as-you-go LLM API keys.
- 📁 **File Support**: Handles file uploads for enhanced data interaction
- 🚀 **One-Click Launch**:  Get started instantly with a simple `auto deep-research` command - **Zero Configuration** needed, truly out-of-the-box experience.


🚀 Own your own personal assistant with much lower cost. Try 🔥Auto-Deep-Research🔥 Now!


## 🔥 News
<div class="scrollable">
    <ul>      
      <li><strong>[2025, April 1]</strong>: &nbsp;🎉🎉 Click to see what Auto-Deepresearch can do! <a href="https://x.com/huang_chao4969/status/1905620201225482264">[Video 1]</a> <a href="https://x.com/huang_chao4969/status/1891676951015981421">[Video 2]</a></li>
      <li><strong>[2025, Feb 16]</strong>: &nbsp;🎉🎉We've cleaned up the codebase of <a href="https://github.com/HKUDS/AutoAgent">AutoAgent</a>, removed the irrelevant parts for Auto-Deep-Research and released the first version of Auto-Deep-Research.</li>
    </ul>
</div>
<span id='table-of-contents'/>

## 📑 Table of Contents

* <a href='#features'>✨ Features</a>
* <a href='#news'>🔥 News</a>
* <a href='#why-to-release-auto-deep-research'>🧐 Why to release Auto-Deep-Research?</a>
* <a href='#quick-start'>⚡ Quick Start</a>
  * <a href='#installation'>Installation</a>
  * <a href='#api-keys-setup'>API Keys Setup</a>
  * <a href='#start-auto-deep-research'>Start Auto-Deep-Research</a>
* <a href='#todo'>☑️ Todo List</a>
* <a href='#documentation'>📖 Documentation</a>
* <a href='#community'>🤝 Join the Community</a>
* <a href='#acknowledgements'>🙏 Acknowledgements</a>
* <a href='#cite'>🌟 Cite</a>

<span id='why-to-release-auto-deep-research'/>

## 🧐 Why to release Auto-Deep-Research?

After releasing AutoAgent (previously known as MetaChain) for a week, we've observed three compelling reasons to introduce Auto-Deep-Research:

1. **Community Interest** 
</br>We noticed significant community interest in our Deep Research alternative functionality. In response, we've streamlined the codebase by removing non-Deep-Research related components to create a more focused tool.

2. **Framework Extensibility**
</br>Auto-Deep-Research serves as the first ready-to-use product built on AutoAgent, demonstrating how quickly and easily you can create powerful Agent Apps using our framework.

3. **Community-Driven Improvements**
</br>We've incorporated valuable community feedback from the first week, introducing features like one-click launch and enhanced LLM compatibility to make the tool more accessible and versatile.

Auto-Deep-Research represents our commitment to both the community's needs and the demonstration of AutoAgent's potential as a foundation for building practical AI applications.

<span id='quick-start'/>

## ⚡ Quick Start

<span id='installation'/>

### Installation

#### Auto-Deep-Research Installation

```bash
conda create -n auto_deep_research python=3.10
conda activate auto_deep_research
git clone https://github.com/HKUDS/Auto-Deep-Research.git
cd Auto-Deep-Research
pip install -e .
```

#### Docker Installation

We use Docker to containerize the agent-interactive environment. So please install [Docker](https://www.docker.com/) first. You don't need to manually pull the pre-built image, because we have let Auto-Deep-Research **automatically pull the pre-built image based on your architecture of your machine**.

<span id='api-keys-setup'/>

### API Keys Setup

Create a environment variable file, just like `.env.template`, and set the API keys for the LLMs you want to use. Not every LLM API Key is required, use what you need.

<span id='start-auto-deep-research'/>

### Start Auto-Deep-Research

#### Command Options:

You can run `auto deep-research` to start Auto-Deep-Research. Some configuration of this command is shown below.

- `--container_name`: Name of the Docker container (default: 'deepresearch')
- `--port`: Port for the container (default: 12346)
- `COMPLETION_MODEL`: Specify the LLM model to use, you should follow the name of [Litellm](https://github.com/BerriAI/litellm) to set the model name. (Default: `claude-3-5-haiku-20241022`)
- `DEBUG`: Enable debug mode for detailed logs (default: False)
- `API_BASE_URL`: The base URL for the LLM provider (default: None)
- `FN_CALL`: Enable function calling (default: None). Most of time, you could ignore this option because we have already set the default value based on the model name.

#### Different LLM Providers

We will show you how easy it is to start Auto-Deep-Research with different LLM providers.

##### Anthropic

* set the `ANTHROPIC_API_KEY` in the `.env` file.

```bash
ANTHROPIC_API_KEY=your_anthropic_api_key
```

* run the following command to start Auto-Deep-Research.

```bash
auto deep-research # default model is claude-3-5-haiku-20241022
```

##### OpenAI

* set the `OPENAI_API_KEY` in the `.env` file.

```bash
OPENAI_API_KEY=your_openai_api_key
```

* run the following command to start Auto-Deep-Research.

```bash
COMPLETION_MODEL=gpt-4o auto deep-research
```

##### Mistral

* set the `MISTRAL_API_KEY` in the `.env` file.

```bash
MISTRAL_API_KEY=your_mistral_api_key
```

* run the following command to start Auto-Deep-Research.

```bash
COMPLETION_MODEL=mistral/mistral-large-2407 auto deep-research
```

##### Gemini - Google AI Studio

* set the `GEMINI_API_KEY` in the `.env` file.

```bash
GEMINI_API_KEY=your_gemini_api_key
```

* run the following command to start Auto-Deep-Research.

```bash
COMPLETION_MODEL=gemini/gemini-2.0-flash auto deep-research
```

##### Huggingface

* set the `HUGGINGFACE_API_KEY` in the `.env` file.

```bash
HUGGINGFACE_API_KEY=your_huggingface_api_key
```

* run the following command to start Auto-Deep-Research.

```bash
COMPLETION_MODEL=huggingface/meta-llama/Llama-3.3-70B-Instruct auto deep-research
```

##### Groq

* set the `GROQ_API_KEY` in the `.env` file.

```bash
GROQ_API_KEY=your_groq_api_key
```

* run the following command to start Auto-Deep-Research.

```bash
COMPLETION_MODEL=groq/deepseek-r1-distill-llama-70b auto deep-research
```

##### OpenAI-Compatible Endpoints (e.g., Grok)

* set the `OPENAI_API_KEY` in the `.env` file.

```bash
OPENAI_API_KEY=your_api_key_for_openai_compatible_endpoints
```

* run the following command to start Auto-Deep-Research.

```bash
COMPLETION_MODEL=openai/grok-2-latest API_BASE_URL=https://api.x.ai/v1 auto deep-research
```

##### OpenRouter (e.g., DeepSeek-R1)

We recommend using OpenRouter as LLM provider of DeepSeek-R1 temporarily. Because official API of DeepSeek-R1 can not be used efficiently.

* set the `OPENROUTER_API_KEY` in the `.env` file.

```bash
OPENROUTER_API_KEY=your_openrouter_api_key
```

* run the following command to start Auto-Deep-Research.

```bash
COMPLETION_MODEL=openrouter/deepseek/deepseek-r1 auto deep-research
```

##### DeepSeek

* set the `DEEPSEEK_API_KEY` in the `.env` file.

```bash
DEEPSEEK_API_KEY=your_deepseek_api_key
```

* run the following command to start Auto-Deep-Research.

```bash
COMPLETION_MODEL=deepseek/deepseek-chat auto deep-research
```

### Tips

#### Import browser cookies to browser environment

You can import the browser cookies to the browser environment to let the agent better access some specific websites. For more details, please refer to the [cookies](./metachain/environment/cookie_json/README.md) folder.

More features coming soon! 🚀 **Web GUI interface** under development.


## ☑️ Todo List

Auto-Deep-Research is continuously evolving! Here's what's coming:

- 🖥️ **GUI Agent**: Supporting *Computer-Use* agents with GUI interaction
- 🏗️ **Code Sandboxes**: Supporting additional environments like **E2B**
- 🎨 **Web Interface**: Developing comprehensive GUI for better user experience

Have ideas or suggestions? Feel free to open an issue! Stay tuned for more exciting updates! 🚀

## 📖 Documentation

A more detailed documentation is coming soon 🚀, and we will update in the [Documentation](https://metachain-ai.github.io/docs) page.

<span id='community'/>

## 🤝 Join the Community

If you think the Auto-Deep-Research is helpful, you can join our community by:

- [Join our Slack workspace](https://join.slack.com/t/metachain-workspace/shared_invite/zt-2zibtmutw-v7xOJObBf9jE2w3x7nctFQ) - Here we talk about research, architecture, and future development.
- [Join our Discord server](https://discord.gg/z68KRvwB) - This is a community-run server for general discussion, questions, and feedback. 
- [Read or post Github Issues](https://github.com/HKUDS/Auto-Deep-Research/issues) - Check out the issues we're working on, or add your own ideas.


<span id='acknowledgements'/>

## 🙏 Acknowledgements

Rome wasn't built in a day. Auto-Deep-Research is built on the [AutoAgent](https://github.com/HKUDS/AutoAgent) framework. We extend our sincere gratitude to all the pioneering works that have shaped AutoAgent, including OpenAI Swarm for framework architecture inspiration, Magentic-one for the three-agent design insights, OpenHands for documentation structure, and many other excellent projects that contributed to agent-environment interaction design. Your innovations have been instrumental in making both AutoAgent and Auto-Deep-Research possible.

<span id='cite'/>

## 🌟 Cite

```tex
@misc{AutoAgent,
      title={{AutoAgent: A Fully-Automated and Zero-Code Framework for LLM Agents}},
      author={Jiabin Tang, Tianyu Fan, Chao Huang},
      year={2025},
      eprint={202502.05957},
      archivePrefix={arXiv},
      primaryClass={cs.AI},
      url={https://arxiv.org/abs/2502.05957},
}
```





