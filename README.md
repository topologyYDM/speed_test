# speed_test

Shell script to test a batch of monocloud / cordcloud nodes' speed

最终要做的事情是通过一个shell脚本文件，一键完成：

  1.  从monocloud / cordcloud爬下订阅的节点的json文件
  2.  依次连接，测速，记录结果
  3.  对结果进行排序并保存
  
# v0.1

  1.  config.json 是某一个节点的信息，已将密码等略去
  2.  speed_test.sh 是核心脚本文件，目前也只是执行两个任务，连接vpn和测速
  3.  out 是目前的一个生成样例

# v0.2

  1. move export.json into /all_config
  2. sh main.sh

# v0.3

  1. 调整了文件组织结构
  2. 节点列表长度(.sh和.py之前传数据)

# v0.4

  1. 把脚本全部改为shell script
  2. ./parse.sh运行，生成out文件，包含所以节点address和测速结果

# v0.5

  1. 可以应对错误节点(包括信息错误和连不上)

***********************************
LICENSE：Code is released under WTFPL.
