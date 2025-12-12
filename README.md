```

docker run -d --name open-webui -p 3000:8080 -v ollama:/root/.ollama -v open-webui:/app/backend/data -e ENABLE_API_KEYS=true ghcr.io/open-webui/open-webui:ollama

http://localhost:3000

API KEY from Open WebUI Settings > Account

Create api-users group, give all permissions, add admin user to group.

model = "llama3"
model_provider = "llama3"

[model_providers.llama3]
name = "llama3:latest"
base_url = "http://localhost:3000/v1"
env_key = "sk-f4e459e17b1c4c38a18b9fb3d02100d6"

```
