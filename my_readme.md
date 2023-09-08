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

### adding missing files to the repo
## add tests 
manually add __test__ folder under src and 

add example.test.js
test('simple test', () => {
  expect(1 + 1).toBe(2);
});

add example.test.js
test('simple test', () => {
  expect(1 + 1).toBe(2);
});

add App.test.js
test('simple test', () => {
  expect(1 + 1).toBe(2);
});

add MovieList.test.js
test('simple test', () => {
  expect(1 + 1).toBe(2);
});

add components folder under src
add blank MovieDetails.js
add blank MovieList.js