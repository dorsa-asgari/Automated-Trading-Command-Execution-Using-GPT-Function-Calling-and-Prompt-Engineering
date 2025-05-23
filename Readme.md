# Milestone 2: NLP command interpretation

This repository is a base example that takes a user prompt and outputs a number of function calls, each corresponding to a specific aspect of Hyperliquid CLI's functionality.

Our model first processes the user's prompt, and if need be, divides the prompt into several subcommands by temporality — I.E. when each subcommand should be executed.

Then, based on the outputted temporal groups and the time to execute each command, each subcommand is then passed onto another request where the subcommand is then converted into a number of function calls which correspond to the predefined functions present in Hyperliquid's CLI.

> To get started and for further explanation, see `Prompt Test.ipynb`.


## Filelist

- `Prompt Test.ipynb`: Executable code is located here, along with prompt examples.
- `ai_utils.py`: Methods for calling and processing API responses.
- `sample_functions.py`: Contains sample functions that *can* be called. Will be replaced with relevant API endpoints by the end of this milestone.
- `.env`: Contains OpenAI API key.
