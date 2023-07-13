# Super Recruiter LLM (in construction) with Open Source LLM Agents

Welcome to the SuperRecruiter LLM utilizing open source LLM agents! This program incorporates cutting-edge technology and automated processes to streamline the recruitment and selection of candidates in the construction industry. By leveraging the Super Recruiter.ai platform and its open source LLM agents, employers can efficiently assess and rank candidates based on their qualifications and responses. This README provides a step-by-step process for utilizing the platform effectively.



<div style="left">
  <a href="https://colab.research.google.com/drive/1AzP33O8rnMW__7ocWJhVBXjKziJXPtim?usp=sharing" target="_blank">
    <img alt="Open In Colab" src="https://colab.research.google.com/assets/colab-badge.svg" />
  </a>
  <a href="https://join.slack.com/t/camel-kwr1314/shared_invite/zt-1vy8u9lbo-ZQmhIAyWSEfSwLCl2r2eKA" target="_blank">
      <img alt="Slack" src="https://img.shields.io/badge/Slack-CAMEL--AI-blueviolet?logo=slack" />
  </a>
  <a href="https://discord.gg/CNcNpquyDc" target="_blank">
    <img alt="Discord" src="https://img.shields.io/badge/Discord-CAMEL--AI-7289da?logo=discord&logoColor=white&color=7289da" />
  </a>
  <a href="https://huggingface.co/camel-ai" target="_blank">
    <img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-CAMEL--AI-ffc107?color=ffc107&logoColor=white" />
  </a>
  <a href="https://twitter.com/CamelAIOrg" target="_blank">
    <img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/CamelAIOrg?style=social&color=brightgreen&logo=twitter" />
  </a>
</div>

# CAMEL: Communicative Agents for “Mind” Exploration of Large Scale Language Model Society

<div align="center">

  <a>![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-brightgreen.svg)</a>
  <a href="https://github.com/camel-ai/camel/actions/workflows/pytest_package.yml">![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/camel-ai/camel/pytest_package.yml?label=tests&logo=github)</a>
  <a href="https://camel-ai.github.io/camel/">
    ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/camel-ai/camel/documentation.yaml?label=docs&logo=github)
  </a>
  <a href="https://github.com/camel-ai/camel/stargazers" target="_blank">
  <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/camel-ai/camel?label=stars&logo=github&color=brightgreen" />
  </a>
  <a href="https://github.com/camel-ai/camel/blob/master/licenses/LICENSE">![License](https://img.shields.io/github/license/camel-ai/camel?label=license&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0IiBmaWxsPSIjZmZmZmZmIj48cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0xMi43NSAyLjc1YS43NS43NSAwIDAwLTEuNSAwVjQuNUg5LjI3NmExLjc1IDEuNzUgMCAwMC0uOTg1LjMwM0w2LjU5NiA1Ljk1N0EuMjUuMjUgMCAwMTYuNDU1IDZIMi4zNTNhLjc1Ljc1IDAgMTAwIDEuNUgzLjkzTC41NjMgMTUuMThhLjc2Mi43NjIgMCAwMC4yMS44OGMuMDguMDY0LjE2MS4xMjUuMzA5LjIyMS4xODYuMTIxLjQ1Mi4yNzguNzkyLjQzMy42OC4zMTEgMS42NjIuNjIgMi44NzYuNjJhNi45MTkgNi45MTkgMCAwMDIuODc2LS42MmMuMzQtLjE1NS42MDYtLjMxMi43OTItLjQzMy4xNS0uMDk3LjIzLS4xNTguMzEtLjIyM2EuNzUuNzUgMCAwMC4yMDktLjg3OEw1LjU2OSA3LjVoLjg4NmMuMzUxIDAgLjY5NC0uMTA2Ljk4NC0uMzAzbDEuNjk2LTEuMTU0QS4yNS4yNSAwIDAxOS4yNzUgNmgxLjk3NXYxNC41SDYuNzYzYS43NS43NSAwIDAwMCAxLjVoMTAuNDc0YS43NS43NSAwIDAwMC0xLjVIMTIuNzVWNmgxLjk3NGMuMDUgMCAuMS4wMTUuMTQuMDQzbDEuNjk3IDEuMTU0Yy4yOS4xOTcuNjMzLjMwMy45ODQuMzAzaC44ODZsLTMuMzY4IDcuNjhhLjc1Ljc1IDAgMDAuMjMuODk2Yy4wMTIuMDA5IDAgMCAuMDAyIDBhMy4xNTQgMy4xNTQgMCAwMC4zMS4yMDZjLjE4NS4xMTIuNDUuMjU2Ljc5LjRhNy4zNDMgNy4zNDMgMCAwMDIuODU1LjU2OCA3LjM0MyA3LjM0MyAwIDAwMi44NTYtLjU2OWMuMzM4LS4xNDMuNjA0LS4yODcuNzktLjM5OWEzLjUgMy41IDAgMDAuMzEtLjIwNi43NS43NSAwIDAwLjIzLS44OTZMMjAuMDcgNy41aDEuNTc4YS43NS43NSAwIDAwMC0xLjVoLTQuMTAyYS4yNS4yNSAwIDAxLS4xNC0uMDQzbC0xLjY5Ny0xLjE1NGExLjc1IDEuNzUgMCAwMC0uOTg0LS4zMDNIMTIuNzVWMi43NXpNMi4xOTMgMTUuMTk4YTUuNDE4IDUuNDE4IDAgMDAyLjU1Ny42MzUgNS40MTggNS40MTggMCAwMDIuNTU3LS42MzVMNC43NSA5LjM2OGwtMi41NTcgNS44M3ptMTQuNTEtLjAyNGMuMDgyLjA0LjE3NC4wODMuMjc1LjEyNi41My4yMjMgMS4zMDUuNDUgMi4yNzIuNDVhNS44NDYgNS44NDYgMCAwMDIuNTQ3LS41NzZMMTkuMjUgOS4zNjdsLTIuNTQ3IDUuODA3eiI+PC9wYXRoPjwvc3ZnPgo=)</a>
</div>

<p align="center">
  
  <a href="https://github.com/camel-ai/camel#installation">Installation</a> |
  <a href="https://camel-ai.github.io/camel/">Documentation</a> |
  <a href="https://github.com/camel-ai/camel/tree/HEAD/examples">Examples</a> |
  <a href="https://arxiv.org/abs/2303.17760">Paper</a> |
  <a href="https://github.com/camel-ai/camel#citation">Citation</a> |
  <a href="https://github.com/camel-ai/camel#contributing-to-camel-">Contributing</a> |
 
</p>

<p align="center">
  <img src='./misc/logo.png' width=800>
</p>

## Overview
The rapid advancement of conversational and chat-based language models has led to remarkable progress in complex task-solving. However, their success heavily relies on human input to guide the conversation, which can be challenging and time-consuming. This paper explores the potential of building scalable techniques to facilitate autonomous cooperation among communicative agents and provide insight into their "cognitive" processes. To address the challenges of achieving autonomous cooperation, we propose a novel communicative agent framework named *role-playing*. Our approach involves using *inception prompting* to guide chat agents toward task completion while maintaining consistency with human intentions. We showcase how role-playing can be used to generate conversational data for studying the behaviors and capabilities of chat agents, providing a valuable resource for investigating conversational language models. Our contributions include introducing a novel communicative agent framework, offering a scalable approach for studying the cooperative behaviors and capabilities of multi-agent systems, and open-sourcing our library to support research on communicative agents and beyond. The GitHub repository of this project is made publicly available on: [https://github.com/camel-ai/camel](https://github.com/camel-ai/camel).


# LLM in Construction with Open Source LLM Agents

Welcome to the LLM in Construction utilizing open source LLM agents! This program incorporates cutting-edge technology and automated processes to streamline the recruitment and selection of candidates in the construction industry. By leveraging the Super Recruiter.ai platform and its open source LLM agents, employers can efficiently assess and rank candidates based on their qualifications and responses. This README provides a step-by-step process for utilizing the platform effectively.

## Documentation

For detailed documentation and usage examples of the CAMEL package used in this project, please refer to the [CAMEL package documentation pages](https://camel-ai.github.io/camel/).

## Installation

To install and set up the required dependencies for the LLM in Construction program, follow the steps below:

1. Create a conda virtual environment:
```
conda create --name camel python=3.10
```

2. Activate the camel conda environment:
```
conda activate camel
```

3. Clone the CAMEL GitHub repository:
```
git clone -b v0.1.0 https://github.com/camel-ai/camel.git
```

4. Change into the project directory:
```
cd camel
```

5. Install CAMEL from source:
```
pip install -e .
```

6. Install pre-commit within the camel environment (only needed for opening pull requests):
```
pip install pre-commit
pre-commit install
```

## Example

To run the LLM in Construction program with the Super Recruiter.ai platform, follow the example below:

1. Add your OpenAI API key to the system environment variables. The method to do this depends on your operating system and shell. Choose the appropriate instructions below:

   **For Bash shell (Linux, macOS, Git Bash on Windows):**
   ```bash
   # Export your OpenAI API key
   export OPENAI_API_KEY=<insert your OpenAI API key>
   ```

   **For Windows Command Prompt:**
   ```cmd
   REM Export your OpenAI API key
   set OPENAI_API_KEY=<insert your OpenAI API key>
   ```

   **For Windows PowerShell:**
   ```powershell
   # Export your OpenAI API key
   $env:OPENAI_API_KEY="<insert your OpenAI API key>"
   ```

   Replace `<insert your OpenAI API key>` with your actual OpenAI API key in each case. Make sure there are no spaces around the `=` sign.

2. After setting the OpenAI API key, run the script:
   ```bash
   # You can change the role pair and initial prompt in role_playing.py
   python examples/ai_society/role_playing.py
   ```

   Customize the role pair and initial prompt in the `role_playing.py` script as per your requirements.

   **Note:** The environment variable is session-specific. If you open a new terminal window or tab, you will need to set the API key again in that new session.

## Benefits of Using Super Recruiter.ai

- **Time-saving:** The automated conversations and evaluation processes significantly reduce the time and effort required for candidate screening and selection. Employers can focus their resources on engaging with the most suitable candidates.

- **Efficient evaluation:** The open source LLM agents enable intelligent conversations, ensuring a thorough evaluation of candidates' abilities and qualifications. This approach enhances the accuracy and reliability of the selection process.

- **Data-driven decisions:** The comprehensive evaluation report generated by Super Recruiter.ai provides employers with valuable data to make informed decisions. The rankings and overview of each candidate facilitate efficient and objective candidate selection.

- **Enhanced candidate experience:** The use of open source LLM agents in the recruitment process creates a dynamic and engaging experience for candidates. The conversational nature of the interviews provides a more realistic representation of their potential performance in the construction industry.

## Getting Started

To get started with the LLM in Construction utilizing open source LLM agents and the Super Recruiter.ai platform, follow these steps:

1. Sign up or log in to the Super Recruiter.ai platform.
2. Upload multiple PDF resumes of candidates into the platform.
3. Let the platform initiate automated conversations with the candidates.
4. Evaluate candidates based on their responses and qualifications.
5. Utilize the comprehensive evaluation report to rank and select top candidates efficiently.

## Requirements

To successfully utilize the Super Recruiter.ai platform and the open source LLM agents for the LLM in Construction, ensure you have the following:

- A modern web browser with internet connectivity.
- PDF resumes of potential candidates.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## Data (Hosted on Hugging Face)
| Dataset | Chat format | Instruction format | Chat format (translated) |
| -- | -- | -- | -- |
| **AI Society** | [Chat format](https://huggingface.co/datasets/camel-ai/ai_society/blob/main/ai_society_chat.tar.gz) | [Instruction format](https://huggingface.co/datasets/camel-ai/ai_society/blob/main/ai_society_instructions.json) | [Chat format (translated)](https://huggingface.co/datasets/camel-ai/ai_society_translated) |
| **Code** | [Chat format](https://huggingface.co/datasets/camel-ai/code/blob/main/code_chat.tar.gz) | [Instruction format](https://huggingface.co/datasets/camel-ai/code/blob/main/code_instructions.json) | x |
| **Math** | [Chat format](https://huggingface.co/datasets/camel-ai/math) | x | x|
| **Physics** | [Chat format](https://huggingface.co/datasets/camel-ai/physics) | x | x |
| **Chemistry** | [Chat format](https://huggingface.co/datasets/camel-ai/chemistry) | x | x |
| **Biology** | [Chat format](https://huggingface.co/datasets/camel-ai/biology) | x | x |

## Visualizations of Instructions and Tasks

| Dataset | Instructions | Tasks |
| -- | -- | -- |
| **AI Society** | [Instructions](https://atlas.nomic.ai/map/3a559a06-87d0-4476-a879-962656242452/db961915-b254-48e8-8e5c-917f827b74c6) | [Tasks](https://atlas.nomic.ai/map/cb96f41b-a6fd-4fe4-ac40-08e101714483/ae06156c-a572-46e9-8345-ebe18586d02b) |
| **Code** | [Instructions](https://atlas.nomic.ai/map/902d6ccb-0bbb-4294-83a8-1c7d2dae03c8/ace2e146-e49f-41db-a1f4-25a2c4be2457) | [Tasks](https://atlas.nomic.ai/map/efc38617-9180-490a-8630-43a05b35d22d/2576addf-a133-45d5-89a9-6b067b6652dd) |
| **Misalignment** | [Instructions](https://atlas.nomic.ai/map/5c491035-a26e-4a05-9593-82ffb2c3ab40/2bd98896-894e-4807-9ed8-a203ccb14d5e) | [Tasks](https://atlas.nomic.ai/map/abc357dd-9c04-4913-9541-63e259d7ac1f/825139a4-af66-427c-9d0e-f36b5492ab3f) |


## News
- Released AI Society and Code dataset (April 2, 2023)
- Initial release of `CAMEL` python library (March 21, 2023)

## Citation
```
@misc{li2023camel,
    title={CAMEL: Communicative Agents for "Mind" Exploration of Large Scale Language Model Society},
    author={Guohao Li and Hasan Abed Al Kader Hammoud and Hani Itani and Dmitrii Khizbullin and Bernard Ghanem},
    year={2023},
    eprint={2303.17760},
    archivePrefix={arXiv},
    primaryClass={cs.AI}
}
```
## Acknowledgement
Special thanks to [Nomic AI](https://home.nomic.ai/) for giving us extended access to their data set exploration tool (Atlas).

We would also like to thank Haya Hammoud for designing the logo of our project.

## License

The intended purpose and licensing of CAMEL is solely for research use.

The source code is licensed under Apache 2.0.

The datasets are licensed under CC BY NC 4.0, which permits only non-commercial usage. It is advised that any models trained using the dataset should not be utilized for anything other than research purposes.
