# chatgpt-retrieval

Simple script to use ChatGPT on your own files.

[YouTube Video](https://youtu.be/9AXP7tCI9PI).

## AWS usage instructions

### 1. Log in to AWS

### 2. Search "EC2" and select "Instances (running)"

### 3. Click on the Instance ID of Chat_bot

### 4. At the top of the screen click "connect', use default config and click "connect".

### 5. In the integrated terminal, cd into Chat_bot folder
```
cd Chat_bot
```
### 6. Create .env file in terminal
```
touch .env
```
### 7. Open .env file and add API Key
```
nano .env
```
Format: OPENAI_API_KEY = 'YOUR-KEY-HERE'
### 8. Install dependencies ([Langchain](https://github.com/hwchase17/langchain)) 
- Only do this the first time you run it.
```
pip install langchain openai chromadb tiktoken unstructured
```

### 9. Test usage (CLI)
OpenAI API:
```
python3 CGPT.py "Who was the first president of the USA?"
```

Test that it is working with your data:
```
python3 CGPT.py "What is my dog's name?"
Output: "The name of your dog is Rex"
```

## Add data

 Place your data into `data/data.txt`.
 - .txt or .csv only