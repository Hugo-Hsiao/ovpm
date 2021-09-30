### 快速安装 ###
from RPM (CentOS/Fedora):

# Add YUM Repo
$ sudo yum install yum-utils -y
$ sudo yum install epel-release -y
$ sudo yum-config-manager --add-repo https://cad.github.io/ovpm/rpm/ovpm.repo

# Install OVPM
$ sudo yum install ovpm

# Enable and start ovpmd service
$ systemctl start ovpmd
$ systemctl enable ovpmd

### 初始化 ###
# We should init the server after fresh install
$ ovpm vpn init --hostname <vpn.example.com> ### 公网IP地址
INFO[0004] ovpm server initialized

# Now, lets create a new vpn user
$ ovpm user create -u hugo -p hugo   ### 创建用户
INFO[0000] user created: hugo
# make user admin                    ### 设置为管理员   
$ ovpm user update -u hugo --admin

### Web 与 VPN 连接访问 ###
OVPM Web Interface can be reached at port :8080 by default.

