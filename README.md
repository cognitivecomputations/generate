This is a demo to showcase Dolphin's ability to generate conversational datasets for training AI with a simple python script.

## Usage

- install ollama

```
ollama pull dolphin-mixtral
pip install ollama
python generate-usecase-chats.py
```

example output:

![image](https://github.com/cognitivecomputations/generate/assets/1117701/d33b0edc-c709-46d8-a489-caedfa7387ba)

There is a reason I'm outputting in this wonky schema.  This schema forces there to be 1 system message, and human/gpt pairs per conversation. 

After generating, you will need convert it to ShareGPT (either [Axolotl style](https://github.com/OpenAccess-AI-Collective/axolotl/blob/main/README.md#conversation) or [LlamaFactory style](https://github.com/hiyouga/LLaMA-Factory/blob/main/data/README.md#:~:text=The%20dataset%20in%20sharegpt%20format%20should%20follow%20the%20below%20format))
