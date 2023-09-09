https://github.com/udacity/cd12354-Movie-Picture-Pipeline/tree/main

## install dependencies
sudo pip3 install pipenv
pipenv install
install nvm:  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
brew install jq
brew install kustomize

## in frontend folder
nvm use
nvm install 18.14
npm ci


npm run lint -- --fix 
- (rerun lint as often as required)


## backend folder
pipenv install flake8

export FLASK_ENV=development

(pipenv install flask-cors) # I think it was not needed in the end

pipenv run serve
