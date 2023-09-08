virtualenv venv
source venv/bin/activate
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
brew install jq
brew install kustomize

### in frontend folder
nvm use
nvm install 18.14
npm ci


npx jest --init
npm run lint -- --fix 
- (rerun lint as often as required)