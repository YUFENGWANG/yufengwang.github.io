---
title: Notes
date: 2017-11-22 20:12:46
tags:
---

# Git:
## .gitignore not working

git rm -r --cached .
## git rename branch

in current branch just type:
git branch -m new-name
## git delete local branch

git branch -d <branch_name>
## git delete remote branch

git push <remote_name> :<branch_name>
## git confict

git push 产生冲突
原因：　本地和远程对同一文件的修改不一致
需要 git pull 然后合并冲突才能push上去
当前更改为本地修改，传入的更改为远端的更改

# Ruby:
## gem

GEM_PATH provides the locations (there may be several) where gems can be found.

GEM_HOME is where gems will be installed (by default).

(Therefore GEM_PATH should include GEM_HOME). 
## erb

<%  %> exexutes the ruby code within the brackets.执行ruby语句
<%= %> print sth into erb file 插值
<% -%> Avoids line break after expression. 避免换行
<%# %> 注释
## rails env

dev: 需要debug gem,
prod: 需要静态资源预处理, js, css的编译压缩
## rake tasks

rake -T: list all rake tasks

rake db:setup
  - rake db:create
  - rake db:schema:load
  - rake db:seed


#  Linux:

## server without any response

1. sudo service nginx status
2. sudo service nginx configtest
3. check port
4. check iptables

## ssh-keygen

ssh-keygen
## adding authorized_keys has no effect

permissions problem
chmod 700 ~/.ssh
chmod 600 ~/.ssh/authorized_keys
chmod go-w ~
## check centos version

rpm --query centos-release
## su -

sudo passwd 
 su -
## 404 with 'Access-Control-Allow-Origin'

check if the url is correct
## tar

  -z : Compress archive using gzip program
  -c: Create archive
  -v: Verbose i.e display progress while creating archive
  -f: Archive File name
  -x: Extract files

  tar -zcvf archive-name.tar.gz directory-name 压缩
  tar -zxvf prog-1-jan-2005.tar.gz　解压
## error code

If a program ended while returning a non-zero value, it means that the program was terminated with some kind of error 非０值有错误。

# Js:
## Uint16Array

16-bit unsigned intergers
blob: binary large object






