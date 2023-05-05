run this in ubantu:

curl http://localhost:8080/v1/completions -H "Content-Type: application/json" -d '{ "model": "vicuna-13B-1.1-GPTQ-4bit-128g.GGML.bin", "prompt": "A long time ago in a galaxy far, far away", "temperature": 0.7 }'


curl http://localhost:8080/v1/completions -H "Content-Type: application/json" -d '{ "model": "gpt4all-lora-quantized-ggml.bin", "prompt": "A long time ago in a galaxy far, far away", "temperature": 0.7 }'


docker run command:
docker run -p 8080:8080 -ti --rm quay.io/go-skynet/local-ai:latest --models-path C:/Users/TuanShu/repos/LocalAI/models/ --context-size 512 --threads 4
