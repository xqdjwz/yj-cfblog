# yj-cfblog
无需服务器，使用cloudflare workers搭建密码发博客,cloudflare KV作为数据库,无其他依赖. 兼容静态博客的速度,以及动态博客的灵活性,方便搭建不折腾.很稳定,
演示地址: https://www.xqdj.site

## 主要特点
使用workers提供的KV作为数据库
使用cloudflare缓存html来降低KV的读写
所有html页面均为缓存,可达到静态博客的速度
使用KV作为数据库,可达到wordpress的灵活性
后台使用markdown语法,方便快捷
一键发布(页面重构+缓存清理)

## 承载能力
KV基本不存在瓶颈,因为使用了缓存,读写很少
唯一瓶颈是 workers的日访问量10w,大约能承受2万IP /日
文章数:1G存储空间,几万篇问题不大

## 搭建教程

## 电脑网页前端演示:
(https://s41.ax1x.com/2026/04/02/peJA5M8.png)

## 手机网页前端演示:
< img src="https://img.xqdj.site/xiazai/mb1.jpg" width="300" alt="图片说明" />
