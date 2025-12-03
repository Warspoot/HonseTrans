# HonseTrans
a silly script for using a LLM to translate silly honse game

## Usage
This repo works best when paired with an lm studio server
### Config
The following Scripts require a config.toml file with parameters:
```
api_url = "http://127.0.0.1:1234/v1/chat/completions"
api_key = "key"
model = "model_name"
temperature = float
nax_tokens = int
top_p = float
top_k = float
repetition_penalty = float
```

### Story Files
Use UmaTL Tools to extract files from the game and place in the raw folder\
It should use a similar format to the "example.json" file\
**run ```py main.py```**

### Character System Text
Find a way to extract the character system text from the game in hachimi format and place it in the root directory with file name "character_system_text.json". Can also add an already existing "character_system_text_dict.json" where the script will avoid duplicate translations and append the new translations to it.\
**run ```py translate_character_system.py```**

