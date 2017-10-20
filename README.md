# ajax load more Demo

## How to start
1. Clone this repository to your local folder
2. Open your terminal, `cd` to target folder, run
```bash
cd sample-ajax
node app.js
```
3. Open your browser, and navigate to `http://localhost:8080/index.html`

## 解释代码
```
__ app.js
__ static
 |__ index.html
```
- `app.js ` 是后端文件，用来创建服务器
- `static` 是静态文件目录
- `index.html` 是静态文件


## todo
window的scroll事件触发频率非常高，应当使用节流机制限制事件处理函数的执行频率，推荐underscore/lodash的throttle函数：
```javascript
window.addEventListener('scroll',_.throttle(eventHandler,200))
```
