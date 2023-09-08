virtualenv venv
source venv/bin/activate
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
brew install jq
brew install kustomize

nvm use
nvm install 18.14
npm ci