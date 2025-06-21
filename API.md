 API.MD
1、大模型名称：MiniMaxAI/MiniMax-M1-80k
2、Api ：开发手册：https://docs.siliconflow.cn/cn/api-reference/chat-completions/chat-completions
3、apikey：sk-lciksnexpylyuxscfkzgzfvmjnhlzzvepwtwxzxvrmyakehg
4、curl --request POST \
  --url https://api.siliconflow.cn/v1/chat/completions \
  --header 'Authorization: Bearer sk-inpjpfsuznsjsaazaswpkapyciqoytabkcopjraghzcjxcoi' \
  --header 'Content-Type: application/json' \
  --data '{
  "model": "MiniMaxAI/MiniMax-M1-80k",
  "stream": false,
  "max_tokens": 512,
  "temperature": 0.7,
  "top_p": 0.7,
  "top_k": 50,
  "frequency_penalty": 0.5,
  "n": 1
}'
{
  "id": "<string>",
  "choices": [
    {
      "message": {
        "role": "assistant",
        "content": "<string>",
        "reasoning_content": "<string>",
        "tool_calls": [
          {
            "id": "<string>",
            "type": "function",
            "function": {
              "name": "<string>",
              "arguments": "<string>"
            }
          }
        ]
      },
      "finish_reason": "stop"
    }
  ],
  "usage": {
    "prompt_tokens": 123,
    "completion_tokens": 123,
    "total_tokens": 123
  },
  "created": 123,
  "model": "<string>",
  "object": "chat.completion"
}
