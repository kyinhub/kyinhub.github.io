﻿---
created: 2022-05-12 15:30
updated: 2022-05-12 17:03
---

<%*
fastStart = async (filename, delayInSecond) => {
if (tp.file.exists(filename)) {
const f = tp.file.find_tfile(filename);
let plugins = (await app.vault.read(f)).split(/\r?\n/);
setTimeout(async () => {
plugins.forEach(async (p) => await app.plugins.enablePlugin(p))
}, delayInSecond * 1000)
}
}
//启动示例库最低插件运行配置启动下面，然后把后面两项的注释掉
await fastStart("FastStart-Plugins-simple", 1)
//正常演示需要启动的插件
//await fastStart("FastStart-Plugins-ShortDelay", 2)
//await fastStart("FastStart-Plugins-LongDelay", 4)
%>
