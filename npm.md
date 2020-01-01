1. List all dependencies: npm list
2. List top level application dependecies: npm list --depth=0
3. View dependency of specific module: 
npm view {module_name},
npm view {module_name} dependencies,
npm view {module_name} versions
4. Find outdated packages: npm outdated
5. Update packages to latest minor & patch: npm update
6. Update to latest major version: npm i -g npm-check-updates && ncu && ncu -u && npm i
7. Outdated global packages: npm -g outdated
8. Publish packages to npm registry: npm adduser && npm login && npm publish && npm version major/minor/patch
