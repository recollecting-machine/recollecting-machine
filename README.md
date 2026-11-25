# Recollecting-Machine
A machine that recollects circumstances of past events.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: What are your recollections of that, machine?" \
  | uvx recollecting-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install recollecting-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
recollecting-machine -a multilogue.txt
```
Or:
```bash
recollecting-machine multilogue.txt > response.txt
```
Or:
```bash
recollecting-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import recollecting_machine
```
