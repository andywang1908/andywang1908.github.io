
## todo

## common mistake

[R1](https://www.toptal.com/nodejs/top-10-common-nodejs-developer-mistakes)

[R2](https://www.airpair.com/node.js/posts/top-10-mistakes-node-developers-make)

[3 Common node.js design patterns that are misused](https://www.appneta.com/blog/3-common-node-js-design-patterns-that-are-misused/)

[Node.js Best Practices](https://blog.risingstack.com/node-js-best-practices/)

[Advanced Error Handling in Node.js With Best Practices](https://www.linkedin.com/pulse/advanced-error-handling-nodejs-best-practices-sandip-das?articleId=7819533121517654217)

## anti pattern

## node_modules

[order](http://www.cnblogs.com/joyeecheung/p/3941705.html)
[some param](http://www.ruanyifeng.com/blog/2016/01/npm-install.html)
[share](http://www.kkh86.com/it/gulp-build-dev-env/guide-sharep-node-modules.html)

##$ watch $apply $digest
[Ref](http://www.angularjs.cn/A0a6)


## interview question
[R1](https://www.toptal.com/nodejs/interview-questions)

## promise

a.cache
b.pressure  crawler
c.excpetion

MEAN（mongodb  + express + angular + node）      Linux, nginx, MySQL, PHP (LEMP) 
如果着眼于现在和未来一段时间的话，建议用Promise，不论是ES6的还是用Q还是用bluebird，毫无疑问立即马上开始用。
如果眼光放长一点看的话，用了co以后基本上再也不愿回去了，即使是“正宫娘娘”Promise。
这co完全就是用yield/generator实现了async/await的效果啊，第一次见的时候，真是有种天马行空的感觉（原谅我见识少）。
它不仅能够“同步非阻塞”，也几乎没有剥夺我对多个非阻塞操作依赖关系或者竞争关系的精确控制，当我需要精确控制异步流程的时候，回去用Promise甚至callback，当我需要写的爽，一泻千里的时候，用async/await（扯远了）。
当然它还有一些不足，这需要实现一个类似C#里的Task库的功能，或者是用别的思路，比如CSP，这真是一个完全打破用观察者的方式来处理GUI事件的新思路，让处理GUI事件变得完全用消息的产生和消费的思路了（又特么扯远了）。
但不管怎样，co提供了一个新的方向，直到Promise，还是“异步”，说到底还是在用“回调”的思路来实现“异步非阻塞”，只是async.js, Promise，它们把回调嵌套“拉平”了，我觉得它们解决的是“回调嵌套的问题”，而不是“回调的问题”。
但到了async/await，包括co模拟出来的，它都打破了“异步”的僵局，实现了“同步非阻塞”，是的这就是大家一直都在说的异步不一定要回调，非阻塞不一定要异步。<del>co，async/await和响马的fibjs一起往go看齐了，难怪tj去搞go去了</del>。

[Concurrency limit in Q promises](http://stackoverflow.com/questions/22366434/concurrency-limit-in-q-promises-node)

## get session id

a.cookie?
b.header?(https://stormpath.com/blog/everything-you-ever-wanted-to-know-about-node-dot-js-sessions)
