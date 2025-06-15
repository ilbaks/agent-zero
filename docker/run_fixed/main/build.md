# For vscode CLI
docker login

# Prerequisites
docker buildx create --name multiarch --driver docker-container --use
docker buildx inspect multiarch --bootstrap

# Creating images
# with hub
should be updated: docker buildx build -f ./Dockerfile.cuda --build-arg BRANCH=baksalyar-dev-main -t ilbaks/agent-zero-run:hacking --platform linux/amd64,linux/arm64 .

# local 
should be updated: docker build -f ./Dockerfile.cuda -t ilbaks/agent-zero-run:hacking --build-arg BRANCH=baksalyar-dev-main --build-arg  .

# Run docker compose
docker compose -f docker-compose.yml up -d
