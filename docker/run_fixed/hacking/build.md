# For vscode CLI
docker login

# Prerequisites
docker buildx create --name multiarch --driver docker-container --use
docker buildx inspect multiarch --bootstrap

# Creating images
# hacking
docker buildx build -f ./DockerfileKali --build-arg BRANCH=baksalyar-dev-main -t ilbaks/agent-zero-run:hacking --platform linux/amd64,linux/arm64 .

# local image from Kali
docker build -f ./DockerfileKali -t ilbaks/agent-zero-run:hacking --build-arg BRANCH=baksalyar-dev-main --build-arg  .

# Run docker compose
docker compose -f docker-compose.yml up -d
