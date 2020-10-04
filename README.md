# web-developer-cheatsheet

## Visual studio code
#### Most Benificial extentions

<a href="https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode" target="_blank"><img src="https://esbenp.gallerycdn.vsassets.io/extensions/esbenp/prettier-vscode/5.7.1/1600972965216/Microsoft.VisualStudio.Services.Icons.Default" height="70" width="70"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=ryu1kn.text-marker" target="_blank"><img src="https://ryu1kn.gallerycdn.vsassets.io/extensions/ryu1kn/text-marker/1.11.0/1555739025789/Microsoft.VisualStudio.Services.Icons.Default" height="70" width="70"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag" target="_blank"><img src="https://formulahendry.gallerycdn.vsassets.io/extensions/formulahendry/auto-rename-tag/0.1.4/1593788476465/Microsoft.VisualStudio.Services.Icons.Default" height="70" width="70"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=thekalinga.bootstrap4-vscode" target="_blank"><img src="https://thekalinga.gallerycdn.vsassets.io/extensions/thekalinga/bootstrap4-vscode/6.1.0/1552290631848/Microsoft.VisualStudio.Services.Icons.Default" height="70" width="70"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer-2" target="_blank"><img src="https://coenraads.gallerycdn.vsassets.io/extensions/coenraads/bracket-pair-colorizer-2/0.2.0/1594062809176/Microsoft.VisualStudio.Services.Icons.Default" height="70" width="70"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=pranaygp.vscode-css-peek" target="_blank"><img src="https://pranaygp.gallerycdn.vsassets.io/extensions/pranaygp/vscode-css-peek/4.0.0/1595892543531/Microsoft.VisualStudio.Services.Icons.Default" height="70" width="70"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=denoland.vscode-deno" target="_blank"><img src="https://denoland.gallerycdn.vsassets.io/extensions/denoland/vscode-deno/2.3.1/1600946310541/Microsoft.VisualStudio.Services.Icons.Default" height="70" width="70"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=ecmel.vscode-html-css" target="_blank"><img src="https://ecmel.gallerycdn.vsassets.io/extensions/ecmel/vscode-html-css/0.2.3/1566473985028/Microsoft.VisualStudio.Services.Icons.Default" height="70" width="70"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=oderwat.indent-rainbow" target="_blank"><img src="https://oderwat.gallerycdn.vsassets.io/extensions/oderwat/indent-rainbow/7.4.0/1552964364054/Microsoft.VisualStudio.Services.Icons.Default" height="70" width="70"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets" target="_blank"><img src="https://xabikos.gallerycdn.vsassets.io/extensions/xabikos/javascriptsnippets/1.8.0/1587489699375/Microsoft.VisualStudio.Services.Icons.Default" height="70" width="70"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer" target="_blank"><img src="https://ritwickdey.gallerycdn.vsassets.io/extensions/ritwickdey/liveserver/5.6.1/1555497731217/Microsoft.VisualStudio.Services.Icons.Default" height="70" width="70"></a>
<a href="https://marketplace.visualstudio.com/items?itemName=bengreenier.vscode-node-readme" target="_blank"><img src="https://bengreenier.gallerycdn.vsassets.io/extensions/bengreenier/vscode-node-readme/3.0.2/1521512283849/Microsoft.VisualStudio.Services.Icons.Default" height="70" width="70"></a>



## NODE
there is no fetch module in node .. so you have to install it but deno it is provided
```
npm i node-fetch --save
```
to use it module use `const fetch = require("node-fetch");` 

to use it globally anywhere use `global.fetch = require("node-fetch");`


## Load testing with Siege
github source code : https://github.com/JoeDog/siege

##### Installation : 
| OS | command | 
| :-----: | :-: |
| mac | `brew install siege` | 
| Debin/Ubuntu | `sudo apt install siege` | 


##### Check version : 

`siege -V`

##### Run : 
```
siege -t2M  -d3 -c150 http://localhost:8080/api/getData 

```
| command param | Meaning | 
| :-----: | :-: |
| -t2M | run for 2 minute | 
| -t2H | run for 2 Hour | 
| -t20S | run for 20 seconds | 
| -d3 | delay for 3 seconds | 
| -c150 | 150 hits  | 


command meaning : Above command will hit 150 hits to server within 3 seconds.
