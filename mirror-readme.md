# vps-tcp-tune（私有镜像）

第三方 VPS TCP/BBR 网络调优脚本的私有备份。

## 来源
- 上游项目: https://github.com/Eric86777/vps-tcp-tune
- 抓取日期: 2026-09-21
- 上游 commit: e5f3e8d262a442b3c3f3167885998a84fdd17136 (2026-09-17T08:47:58Z)

## 文件
- install-alias.sh — 为主脚本创建 bbr 快捷别名（写进 .bashrc/.zshrc）
- net-tcp-tune.sh — 主调优脚本（BBR/队列/内核参数一键调优）

## 用途记录
- 已在其中一台 VPS 手动启用 BBR + fq（sysctl 持久化），未使用本脚本的别名方式。

## 更新方法
1. 查上游最新 commit: curl -s https://api.github.com/repos/Eric86777/vps-tcp-tune/commits/main | grep sha
2. 与上面记录的 commit 对比；有更新则重新下载两个文件，diff 审查后提交本仓库
