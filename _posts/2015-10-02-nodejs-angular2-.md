
## common mistake

## anti pattern.

## component

[Comparison of Kendo UI and Wijmo](http://erictopia.com/2012/07/comparison-of-kendo-ui-and-wijmo-part-1/)

图片视频类 输入控件类 文本编辑器 界面类(页内滚动工具 树状目录组织扩展)
[AngularJS常用插件与指令收集](https://chensd.com/2015-06/AngularJS-popular-Plugins-and-Directive.html)

## version

[~ ^](http://blog.kankanan.com/article/package.json-65874ef6-dependencies-4e2d7684540479cd7248672c53f75f625f0f.html)

## problem

## doc

[TypeScript Handbook](https://zhongsp.gitbooks.io/typescript-handbook/content/doc/handbook/tutorials/Angular%202.html)
[十条](http://www.10tiao.com/html/283/201702/2650862488/1.html)

## unit test

TDD  karma,Jasmin
BDD  Mocha,Chai

## vs react

[我由Angular转向React](http://www.iteye.com/news/30249)


## notes
```

https://www.npmjs.com/package/ng2-redux-router

http://stackoverflow.com/questions/35326689/how-to-catch-exception-correctly-from-http-request

https://medium.com/@arnaudrinquin/build-modular-application-with-npm-local-modules-dfc5ff047bcc#.z7mxs3tmv

http://stackoverflow.com/questions/15806241/how-to-specify-local-modules-as-npm-package-dependencies

npm install ../s2i-common-rest/

error handle + log4ts
project seperate

var mockData = require('assets/mock-data/mock-data.json');

//come compile erro because of mocha check code coved percentage
    reporters: [ 'mocha', 'coverage' ],

https://help.ubuntu.com/community/How%20to%20Create%20a%20Network%20Share%20Via%20Samba%20Via%20CLI%20(Command-line%20interface/Linux%20Terminal)%20-%20Uncomplicated,%20Simple%20and%20Brief%20Way!

[share]
path = /home/andy/share
valid users = root
read only = no

    "iac": {
        "getOrderItem": "/api/s2i/iac/api/v1/orderitems/",
        "verify": "/api/s2i/iac/api/v1/providers/"
        "addToCart": "/api/s2i/iac/api/v1/carts/",
        "saveUpdate": "/api/s2i/iac/api/v1/carts/",
    }

log4ts monitor wcm           translation

%AppData%\npm\node_modules


npm install -g typescript
npm install -g typings

---maybe---
npm install marked@0.3.6 -g
npm install node-gyp@3.4.0 -g


angular v1:
3.? active windows by active online and cancel?

v2:
0.svn client
1.chrome

v3:
0.verify vm setting
1.
--npm install -g typescript
--npm install -g typings

set HTTP_PROXY=http://204.40.194.129:3128
set HTTPS_PROXY=http://204.40.194.129:3128
SET SASS_BINARY_PATH=C:/green/0trans/win32-x64-48_binding.node

npm install -g angular-cli  -- must after typescript and typings behind proxy, otherwise some sass error will pop up


2.download svn

https://gscbiqdcapmdw01.cihs.ad.gov.on.ca:8443/svn/SOIT_S2I_Portal/branches/angular2/s2i-angular2-v1


---------------from comm-rest to build,this version is not working!!!!!!!!
    "to-string-loader": "^1.1.4",
npm install to-string-loader@^1.1.4

    "@types/express": "4.0.32",
npm install @types/express@4.0.32
    "@types/source-map": "^0.1.27",
npm install @types/source-map@^0.1.27


npm update    still not working on ts step.
-------


---  TypeError: Cannot read property 'exclude' of undefined
npm uninstall typescript
npm uninstall awesome-typescript-loader
npm install typescript@2.0.10
npm install awesome-typescript-loader@^2.2.1

npm install redux-localstorage --save    why?


update issue:
  //constructor(private ngRedux: NgRedux < any > , private iacClient: IacClient) {}
in W:\document\nodejs\V1\s2i-common-rest\src\app\quote\actions\iac.actions.ts
resolved:       TODO support timeout
//.timeout(10000, this.throwError('timeout123'))

  //ngRedux.connect(this.mapStateToTarget, this.mapDispatchToThis)(this);
in W:\document\nodejs\V1\s2i-common-rest\src\app\app.component.ts
resolved:
    this.ngRedux
	  .select(state=>state.iacState)
	  .subscribe(newValue=> this.iacState = newValue );

http://10.160.200.212:4200/api/s2i/iac/api/v1/orderitems/abcd
http://10.160.200.184:10039/api/s2i/iac/api/v1/orderitems/abcd

F:\new year\chris-vision\s2i-common-rest\config\webpack.dev.js:
proxy: {
   "/api/*": {
      "target": "http://10.160.200.184:10039",
      "secure": false
   }
}

https://markdowncss.github.io/   markdown css

https://github.com/angularclass/angular2-webpack-starter
http://stackoverflow.com/questions/5259276/intellij-idea-10-generate-entity-pojo-from-db-model


phase 2
npm install awesome-typescript-loader@^2.2.4 --save    must 2.2.4 for ForkCheckerPlugin
npm install script-ext-html-webpack-plugin@^1.4.1 --save   

npm install angular2-router-loader@^0.3.4 --save   
npm install angular2-template-loader@^0.6.0 --save   


https://medium.com/@isaacplmann/getting-your-angular-2-library-ready-for-aot-90d1347bcad#.yiwuccyss
https://github.com/qdouble/angular-webpack2-starter
https://medium.com/@cyrilletuzi/how-to-build-and-publish-an-angular-module-7ad19c0b4464#.9tekj2qr3


todo:
blog  css  input
tunning package install warning
lint warning
run index.html error map.missing
compress error
(almost done)do not use http-server for proxy reason          
make it more smaller
where is js--map,how to use it to debug
specific version?



import 'core-js';
import 'reflect-metadata';
import 'zone.js/dist/zone';

put into header in vendor.ts


import 'core-js';
import 'reflect-metadata';
import 'zone.js/dist/zone';

import './polyfills.ts';
in main.ts    for     Cannot resolve all parameters for 'Parser'(?)
https://github.com/angular/angular/issues/13609

http://10.160.200.135:6060/app/s2i-common-rest/index.html  is working 

```

## usage

### abc

