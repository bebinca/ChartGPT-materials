# Prompt to generate abstract utterance

We used GPT-3 (text-davinci-003) to generate abstract utterances from the original utterances in nvBench. 

Prompt: 

```
This is a table named {{table name}}: 
{{table data in CSV}}
We have a tool to automatically draw charts according to your utterances and the table data. 
Now we have a clear and explicit utterance example:
{{the original utterance from nvBench}}
We want to use more abstract utterances to test the tool's ability to understand natural language, as users always give utterances that is not so explicit and clear. 
Please rewrite a new abstract utterance based on the given utterance. The new utterance should be more natural, vague, and incomplete. Rewrite it into a
[For query] {short query consists of some keywords}.
[For question] {question ends with a question mark}.
[For command] {command that directly tells the system to do what}.
```

Accommodate different phrasings by selecting the `For query / For question / For command` options. 
