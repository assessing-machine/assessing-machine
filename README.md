# Assessing-Machine
A machine that assesses possible outcomes.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: What is your assessment, machine?" \
  | uvx assessing-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install assessing-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
assessing-machine -a multilogue.txt
```
Or:
```bash
assessing-machine multilogue.txt > response.txt
```
Or:
```bash
assessing-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import assessing_machine
```
