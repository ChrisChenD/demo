# https://nodejs.org/en/download/package-manager/
# https://github.com/nodesource/distributions/blob/master/README.md#debinstall
# install node
curl -fsSL https://deb.nodesource.com/setup_17.x | sudo -E bash -
sudo apt-get install -y nodejs
# install next.js package
npx create-next-app@latest create_test
cd create_test
npm run dev


