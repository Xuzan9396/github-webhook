# github-webhook
github 自动挂钩
Gitlab 方式
下载项目

git clone https://github.com/dounine/gitlab-webhook.git
自行修改第9行读取密码文件的位置

fs.readFile('/root/issp/gitlab-webhook/password.txt', 'utf8',....
修改第65行执行shell脚本位置

cmd.get('/root/issp/docker/' + event.mode + '/run.sh',....
运行

cd gitlab-webhook && ./start.sh
gitlab配置

URL：http://xxxxx:7777/webhook
Secret Token：password.txt里面的密码
Github 方式
下载项目

git clone https://github.com/dounine/github-webhook.git
自行修改第3行密码文件的位置

var secretPassword = 'abc123' //github secret安全密码
修改第7行执行shell脚本位置

var bash = '/root/xxx/test.sh' //执行的脚本
运行

cd github-webhook && ./start.sh
gitlab配置

Payload URL：http://xxxxx:7777/webhook
Secret：安全密码


链接：<a href='https://www.jianshu.com/p/d36cf005529a'>https://www.jianshu.com/p/d36cf005529a</a>
