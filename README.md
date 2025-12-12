```

docker run -d --name open-webui -p 3000:8080 -v ollama:/root/.ollama -v open-webui:/app/backend/data -e ENABLE_API_KEYS=true ghcr.io/open-webui/open-webui:ollama

http://localhost:3000

API KEY from Open WebUI Settings > Account

model = "ollama3"
model_provider = "ollama3"

[model_providers.ollama3]
name = "Ollama"
base_url = "http://localhost:3000/v1"
env_key = "API KEY from Open WebUI Settings > Account"

```
