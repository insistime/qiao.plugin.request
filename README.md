# urls
## homepage
[https://code.insistime.com/qiao.plugin.request](https://code.insistime.com/qiao.plugin.request)

## github
[https://github.com/insistime/qiao.plugin.request](https://github.com/insistime/qiao.plugin.request)

## npm
[https://www.npmjs.com/package/qiao.plugin.request](https://www.npmjs.com/package/qiao.plugin.request)

# started
## install
npm install qiao.plugin.request

## dependencies
1. http request by request

## documentation
1. request, https://www.npmjs.com/package/request

# api
## getSync
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = async function(){
	try{
		var url = 'http://www.baidu.com';
		var res = await qiaoPluginRequest.getSync({
			url	: url,
			qs	: {
				test : 'test'
			}
		});
		
		console.log(res);
	}catch(e){
		console.log(e);
	}
};

test(); 
```

## postSync
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = async function(){
	try{
		var url = 'http://www.baidu.com';
		var res = await qiaoPluginRequest.postSync({
			url	: url,
			qs	: {
				test : 'test'
			}
		});
		
		console.log(res);
	}catch(e){
		console.log(e);
	}
};

test();
```

## putSync
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = async function(){
	try{
		var url = 'http://10.33.12.68:8002/put';
		var res = await qiaoPluginRequest.putSync({
			url	: url
		});
		
		console.log(res);
	}catch(e){
		console.log(e);
	}
};

test();
```

## patchSync
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = async function(){
	try{
		var url = 'http://10.33.12.68:8002/patch';
		var res = await qiaoPluginRequest.patchSync({
			url	: url
		});
		
		console.log(res);
	}catch(e){
		console.log(e);
	}
};

test();
```

## deleteSync
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = async function(){
	try{
		var url = 'http://10.33.12.68:8002/delete';
		var res = await qiaoPluginRequest.deleteSync({
			url	: url
		});
		
		console.log(res);
	}catch(e){
		console.log(e);
	}
};

test();
```

## headSync
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = async function(){
	try{
		var url = 'http://10.33.12.68:8002/head';
		var res = await qiaoPluginRequest.headSync({
			url	: url
		});
		
		console.log(res);
	}catch(e){
		console.log(e);
	}
};

test();
```

## get
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = function(){
	var url = 'http://www.baidu.com';
	qiaoPluginRequest.get({
		url	: url,
		qs	: {
			test : 'test'
		}
	}, function(err, rs, body){
		console.log(err, body);
	});
};

test();
```

## post
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = function(){
	var url = 'http://www.baidu.com';
	qiaoPluginRequest.post({
		url	: url,
		qs	: {
			test : 'test'
		}
	}, function(err, rs, body){
		console.log(err, body);
	});
};

test();
```

## put
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = function(){
	var url = 'http://10.33.12.68:8002/put';
	qiaoPluginRequest.put({
		url	: url
	}, function(err, rs, body){
		console.log(err, body);
	});
};

test();
```

## patch
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = function(){
	var url = 'http://10.33.12.68:8002/patch';
	qiaoPluginRequest.patch({
		url	: url
	}, function(err, rs, body){
		console.log(err, body);
	});
};

test();
```

## delete
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = function(){
	var url = 'http://10.33.12.68:8002/delete';
	qiaoPluginRequest.delete({
		url	: url
	}, function(err, rs, body){
		console.log(err, body);
	});
};

test();
```

## head
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = function(){
	var url = 'http://10.33.12.68:8002/head';
	qiaoPluginRequest.head({
		url	: url
	}, function(err, rs, body){
		console.log(err, rs.headers);
	});
};

test();
```

## download
```javascript
'use strict';

var qiaoPluginRequest = require('qiao.plugin.request');

var test = async function(){
	try{
		var url 	= 'https://www.baidu.com/img/bd_logo1.png';
		var path	= 'd:/test.png';
		
		await qiaoPluginRequest.download(url, path);
	}catch(e){
		console.log(e);
	}
};

test();
```

# version
## 0.1.0.20190117
1. add download
2. donwload finish

## 0.0.9.20190107
1. modify desc
2. update request@2.88.0

## 0.0.8.20181127
1. modify method name
2. add .js

## 0.0.7.20181122
1. npm audit fix

## 0.0.6.20180720
1. https homepage

## 0.0.5.20180719
1. modify readme.md

## 0.0.4.20180523
1. npm audit

## 0.0.3.20180511
1. npm audit

## 0.0.2.20180210
1. delete reqwest
2. highlight md

## 0.0.1.20180208
1. init project
2. request get
3. request post
4. modify index.js