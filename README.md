# 作业链接

https://www.cnblogs.com/lxbxyz/p/12489202.html

# 结对学号

- 021700915
- 091700403

# 项目介绍

该项目利用HTML展示页面，node.js爬取并处理数据，向用户展示了全国疫情的状态，包括地图的高亮设计，曲线图展示全国的确诊、疑似、治愈、死亡总人数和新增人数，以及各省份的各个趋势图。

# 如何构建项目

1. 下载`node.js`
2. 安装yarn：打开命令行输入 `npm install -g yarn`
3. 在该项目的server文件夹下下载superagent，cheerio：`yarn add superagent cheerio`
4. 在该项目的server文件夹下下载express：`yarn add express`
5. 在server文件夹下，按住shift+鼠标左键，点击打开PowerShell窗口，输入`node index.js`运行
6. 用浏览器打开country.html或specific.html即可看到效果