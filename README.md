docker run -d \                
  --name open-webui \
  -p 3000:8080 \
  -v ollama:/root/.ollama \
  -v open-webui:/app/backend/data \
  -e ENABLE_API_KEYS=true     \ 
  ghcr.io/open-webui/open-webui:ollama
