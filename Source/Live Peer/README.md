<p align="center">
  <img height="100" height="auto" src="https://raw.githubusercontent.com/Nodeist/Kurulumlar/main/logos/source.png">
</p>


# Source Live Peers
Here is a list of active peers. Add them to your `config.toml` if you have trouble finding peers.
```
d0bf1f313c3fe5d9e890f7754950238493497211@62.171.178.217:26656,bdf9b6ad38b803358e7fd99f35b14795ebcd8144@190.2.155.67:29656,0329379c13d72b6146915ec9b60201d8170cc99c@157.245.33.21:26656,d57c4825b2823f94f87b7cbcc4748420edfcd6df@5.161.77.35:26656,8f283e5d395f858da9665faf4214a85aaa8e171f@95.216.218.186:26656,08e5694cbc077e361cc2e9daa7f91aa67797c92e@65.109.85.170:34656,af73c866e08fc8a789d247dc0694b5117328131d@34.89.201.124:26656,06885ec73c228de552c4120ab50c78152b20fc9d@162.19.92.92:26656,246686b1e8c06ead485377c03568cb9f1db3917d@176.9.19.48:26686,6ca675f9d949d5c9afc8849adf7b39bc7fccf74f@164.92.98.17:26656,a2a553a7ac782bb1d9b265abaf19dee339b50529@135.181.1.109:28656,cb09ec2e5dc91beaa3d05c79a0a8d6c30fffcc59@194.163.175.208:26656,3787aeaa6585ec6ff9c09746fdb28630f0d659cb@3.81.88.66:26656,866c35beaae2aafaebc328035e2deb9290da0b7a@38.242.241.111:26656,08f192a375c18dea003651f6f6ee9065a09585e9@45.67.32.53:36656,5c2a752c9b1952dbed075c56c600c3a79b58c395@95.214.55.232:26966,c749b47c438842d9874b515de130dfb11431360f@147.182.211.27:26656,383a0684aadfe507e097c36b34d6243da59d9ed5@207.180.232.91:26656,49b025c08193c8846956423ac80504b0bab2b777@185.182.187.239:26656,56bc68608258208e32eb20d66785eab4b5b5a82a@65.108.238.217:11164,76894391ff3fb5937654758b12d1eecd69eb943e@161.97.151.64:26656,34f06c7b70d301f8b703c8a42e512157c4947b43@78.185.53.253:26656,b958d18452ec5458323606d934906cc90d462203@194.233.93.124:26656,b5cfe488ddf0b9e902716b2e18686f8b13c03182@62.171.181.251:26656,c0dd01d86ed19becc998874a6a2152513b41f34d@45.84.138.66:28656
```

Here is a script for you to update `persistent_peers` setting with these peers in `config.toml`.

```
PEERS=d0bf1f313c3fe5d9e890f7754950238493497211@62.171.178.217:26656,bdf9b6ad38b803358e7fd99f35b14795ebcd8144@190.2.155.67:29656,0329379c13d72b6146915ec9b60201d8170cc99c@157.245.33.21:26656,d57c4825b2823f94f87b7cbcc4748420edfcd6df@5.161.77.35:26656,8f283e5d395f858da9665faf4214a85aaa8e171f@95.216.218.186:26656,08e5694cbc077e361cc2e9daa7f91aa67797c92e@65.109.85.170:34656,af73c866e08fc8a789d247dc0694b5117328131d@34.89.201.124:26656,06885ec73c228de552c4120ab50c78152b20fc9d@162.19.92.92:26656,246686b1e8c06ead485377c03568cb9f1db3917d@176.9.19.48:26686,6ca675f9d949d5c9afc8849adf7b39bc7fccf74f@164.92.98.17:26656,a2a553a7ac782bb1d9b265abaf19dee339b50529@135.181.1.109:28656,cb09ec2e5dc91beaa3d05c79a0a8d6c30fffcc59@194.163.175.208:26656,3787aeaa6585ec6ff9c09746fdb28630f0d659cb@3.81.88.66:26656,866c35beaae2aafaebc328035e2deb9290da0b7a@38.242.241.111:26656,08f192a375c18dea003651f6f6ee9065a09585e9@45.67.32.53:36656,5c2a752c9b1952dbed075c56c600c3a79b58c395@95.214.55.232:26966,c749b47c438842d9874b515de130dfb11431360f@147.182.211.27:26656,383a0684aadfe507e097c36b34d6243da59d9ed5@207.180.232.91:26656,49b025c08193c8846956423ac80504b0bab2b777@185.182.187.239:26656,56bc68608258208e32eb20d66785eab4b5b5a82a@65.108.238.217:11164,76894391ff3fb5937654758b12d1eecd69eb943e@161.97.151.64:26656,34f06c7b70d301f8b703c8a42e512157c4947b43@78.185.53.253:26656,b958d18452ec5458323606d934906cc90d462203@194.233.93.124:26656,b5cfe488ddf0b9e902716b2e18686f8b13c03182@62.171.181.251:26656,c0dd01d86ed19becc998874a6a2152513b41f34d@45.84.138.66:28656
sed -i.bak -e "s/^persistent_peers *=.*/persistent_peers = \"$PEERS\"/" $HOME/.source/config/config.toml
```