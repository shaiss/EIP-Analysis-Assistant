# Ethereum Improvement Proposal (EIP) Analysis Assistant

[![GitHub stars](https://img.shields.io/github/stars/shaiss/EIP-Analysis-Assistant.svg?style=social&label=Star&maxAge=2592000)](https://github.com/shaiss/EIP-Analysis-Assistant/stargazers/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An intelligent analysis tool built with Dify that evaluates Ethereum Improvement Proposals across multiple dimensions, providing comprehensive insights for developers, researchers, and the Ethereum community.

## 🚀 Features

The EIP Assistant evaluates proposals across five key dimensions:

- **Technical Difficulty**: Assesses implementation complexity on a scale of 100-400
- **Novelty**: Scores how innovative the proposal is on a scale of 1-10
- **Ethereum Impact**: Evaluates potential effects on the Ethereum ecosystem (1-10)
- **Polygon/L2 Impact**: Analyzes implications for Layer 2 solutions like Polygon (1-10)
- **Community Engagement**: Measures the level of developer and community involvement (1-10)

## 📊 How It Works

1. **Input**: Provide an EIP URL or number
2. **Analysis**: The assistant fetches the EIP content and discussion threads
3. **Multi-Model Evaluation**: Uses a combination of GPT-4, Claude, and Gemini models for balanced analysis
4. **Comprehensive Report**: Generates a markdown report with:
   - TLDR summary of key findings
   - Visual score summary table
   - Detailed analysis for each dimension
   - Supporting evidence from EIP documents and discussions

## 🛠️ Technology Stack

This assistant is built using [Dify](https://dify.ai/), an LLM application development platform, with:

- **Multiple AI Models**:
  - Claude 3.5 Sonnet
  - GPT-4o and GPT-4o Mini
  - Gemini 1.5 Pro and Flash
- **Web Scraping**: Jina Reader for fetching EIP content and discussions
- **Workflow Engine**: Custom multi-step workflow with parameter extraction and analysis

## 📋 Use Cases

- **Developers**: Quickly assess the complexity and potential impact of proposed Ethereum changes
- **Researchers**: Analyze innovation patterns in the Ethereum ecosystem
- **Investors**: Understand the significance of upcoming protocol changes
- **Contributors**: Identify high-impact, high-engagement proposals worth contributing to

## 🔧 Installation & Setup

1. Clone this repository 
2. Import the `eip-assistant.yml` workflow into your Dify instance:
   ```
   dify import eip-assistant.yml
   ```
3. Configure your API keys for OpenAI, Anthropic, and Google in your Dify settings
4. Deploy the assistant to your preferred environment

## 📖 Usage Example

```
Input: "EIP-1559"

Output:
# EIP Analysis Report

## TLDR
EIP-1559 introduces a significant change to Ethereum's fee mechanism, burning base fees to improve user experience and introduce deflationary pressure. It's highly novel (8/10), technically challenging (320/400), and has substantial impact on Ethereum (9/10) and Layer 2 solutions (7/10), with exceptional community engagement (9/10).

## Summary Table
| Aspect | Score | Assessment |
|--------|-------|------------|
| Technical Difficulty | 320/400 | High |
| Novelty | 8/10 | Very Innovative |
| Ethereum Impact | 9/10 | Major Impact |
| L2/Polygon Impact | 7/10 | Significant |
| Community Engagement | 9/10 | Highly Active |

...
```

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/yourusername/eip-assistant/issues).

## 🙏 Acknowledgements

- The Ethereum Foundation and EIP authors
- [Dify.AI](https://dify.ai/) for the workflow platform
- All contributors to this project

---

Built with ❤️ for the Ethereum community
