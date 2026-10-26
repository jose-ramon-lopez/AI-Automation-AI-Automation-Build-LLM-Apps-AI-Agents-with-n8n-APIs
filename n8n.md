# N8N

## Instalar
Instalo nodejs https://nodejs.org/en/download

```bash
# instalo nvm
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash

# añado esto a ~/.bashrc
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion


# recargo la shell
source ~/.bashrc

# compruebo que está instalado
vm --version
0.40.3

# instalo nodejs 24 (para ejecutar javascript)
nvm install 24
Downloading and installing node v24.22.1...
Downloading https://nodejs.org/dist/v24.22.1/node-v24.22.1-linux-x64.tar.xz...
################################################################################################################################################################################################### 100.0%
Computing checksum with sha256sum
Checksums matched!


# por si tengo mas versiones la pongo por defecto
# miro las versiones que tengo
nvm list
nvm alias default 24

# veo que tengo nodejs
node --version
v24.22.1

# veo que tengo instalado npm (es el gestor de paquetes de nodejs)
npm -v
11.19.1

# instalo n8n
npm install -g n8n
...
npm warn deprecated @opentelemetry/sdk-trace-base@2.7.1: Use @opentelemetry/sdk-trace package
npm warn deprecated @langchain/community@0.0.57: This package has been deprecated. See https://github.com/langchain-ai/langchainjs-community/issues/61 for more info
npm warn deprecated @langchain/community@1.1.27: This package has been deprecated. See https://github.com/langchain-ai/langchainjs-community/issues/61 for more info
npm warn deprecated @langchain/community@1.1.27: This package has been deprecated. See https://github.com/langchain-ai/langchainjs-community/issues/61 for more info

added 2331 packages in 4m

368 packages are looking for funding
  run `npm fund` for details
npm warn install-scripts 16 packages have install scripts not yet covered by allowScripts:
npm warn install-scripts   @parcel/watcher@2.6.0 (install: node scripts/build-from-source.js)
npm warn install-scripts   isolated-vm@7.0.1 (install: node-gyp-build 'node-gyp rebuild -j 4 --release -v' || node-gyp rebuild --release -j max)
npm warn install-scripts   sqlite3@5.1.7 (install: prebuild-install -r napi || node-gyp rebuild)
npm warn install-scripts   protobufjs@7.6.6 (postinstall: node scripts/postinstall)
npm warn install-scripts   agent-browser@0.26.0 (postinstall: node scripts/postinstall.js)
npm warn install-scripts   oracledb@6.10.0 (install: node package/install.js)
npm warn install-scripts   msgpackr-extract@3.0.4 (install: node-gyp-build-optional-packages)
npm warn install-scripts   ssh2@1.15.0 (install: node install.js)
npm warn install-scripts   @sentry/node-native-stacktrace@0.5.2 (install: node scripts/check-build.mjs)
npm warn install-scripts   @sentry/node-cpu-profiler@2.4.4 (install: node scripts/check-build.js)
npm warn install-scripts   @confluentinc/kafka-javascript@1.9.1 (install: node-pre-gyp install --fallback-to-build)
npm warn install-scripts   cpu-features@0.0.10 (install: node buildcheck.js > buildcheck.gypi && node-gyp rebuild)
npm warn install-scripts   ssh2@1.17.0 (install: node install.js)
npm warn install-scripts   @scarf/scarf@1.4.0 (postinstall: node ./report.js)
npm warn install-scripts   vue-demi@0.14.10 (postinstall: node -e "try{require('./scripts/postinstall.js')}catch(e){}")
npm warn install-scripts   vue-demi@0.14.10 (postinstall: node -e "try{require('./scripts/postinstall.js')}catch(e){}")
npm warn install-scripts
npm warn install-scripts Run `npm install -g --allow-scripts=@parcel/watcher,isolated-vm,sqlite3,protobufjs,agent-browser,oracledb,msgpackr-extract,ssh2,@sentry/node-native-stacktrace,@sentry/node-cpu-profiler,@confluentinc/kafka-javascript,cpu-features,ssh2,@scarf/scarf,vue-demi,vue-demi` to allow these scripts once, or `npm config set allow-scripts=@parcel/watcher,isolated-vm,sqlite3,protobufjs,agent-browser,oracledb,msgpackr-extract,ssh2,@sentry/node-native-stacktrace,@sentry/node-cpu-profiler,@confluentinc/kafka-javascript,cpu-features,ssh2,@scarf/scarf,vue-demi,vue-demi --location=user` to allow them for all global installs.
jose@jose:~$ 


# arranco n8n
n8n start

# relleno los datos
http://localhost:5678/setup


# actualizo n8n
npm update -g n8n

```

https://github.com/n8n-io/n8n



## n8n online
tiene mas opciones
https://n8n.io/



## Primera automatización   
