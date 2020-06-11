都是一直使用一键脚本，但是，怕出现意外情况失效，（比如删库）多会一个方式，也是多一种预防，找到了这个资料：

已经写好apx.php，直接下载文件到机器上：

下载文件地址：https://www.vrrmr.net/55R/apx.php

使用ifconfig命令查看当前机器MAC地址，然后执行以下命令：

php apx.php mac expireYear bandwidth

例如：php apx.php 02:42:ac:11:46:9e 2999 0 bandwidth=0代表无限制，执行后将会在当前目录生成文件名为apx-29991231.lic的授权文件。 同时，请记录下执行后生成的SerialNo。

选择对应的Linux版本后，下载对应的锐速离线安装包并解压。

将第一步生成的lic授权文件放入apxfiles/etc文件夹，同时编辑该目录下的config文件，修改文件尾部以下部分：

修改完成后，将安装文件打包上传至服务器，在服务器解压后执行：
bash install.sh

接下来的安装步骤与锐速官方的安装文件相同，在此不再赘述。

注意： 安装完成后，请执行 chattr +i /serverspeeder/etc/apx* ，防止锐速联网更新授权文件导致带宽变回20M。


# 启动命令：
/appex/bin/lotServer.sh start
# 停止加速：
/appex/bin/lotServer.sh stop
# 状态查询：
/appex/bin/lotServer.sh status
# 重新启动：
/appex/bin/lotServer.sh restart


bash <(wget --no-check-certificate -qO-  https://git.io/lotServerInstall.sh) install 2.6.32-573.1.1.el6.x86_64
bash <(wget --no-check-certificate -qO-  https://git.io/lotServerInstall.sh) install 4.20.11-1.el7.elrepo.x86_64

Amazon / 14.03 / 3.10.35-43.137.amzn1.x86_64 / 64-bits
Amazon / 2014.09 / 3.14.19-17.43.amzn1.x86_64 / 64-bits
Amazon / 2015.09 / 3.10.42-52.145.amzn1.x86_64 / 64-bits
Amazon / 2015.09 / 3.14.48-33.39.amzn1.x86_64 / 64-bits
Amazon / 2015.09 / 4.1.10-17.31.amzn1.x86_64 / 64-bits
Amazon / 2015.09 / 4.1.13-19.30.amzn1.x86_64 / 64-bits
Amazon / 2015.09 / 4.1.17-22.30.amzn1.x86_64 / 64-bits
Amazon / 2015.09 / 4.1.7-154.234.amzn1.x86_64 / 64-bits
Amazon / 2018.03 / 4.4.11-23.53.amzn1.x86_64 / 64-bits
CentOS / 5 / 2.6.18-164.el5pae / 32-bits
CentOS / 5 / 2.6.18-308.4.1.el5xen / 64-bits
CentOS / 5 / 2.6.18-53.el5 / 32-bits
CentOS / 5 / 2.6.18-53.el5 / 64-bits
CentOS / 5 / 2.6.18-53.el5xen / 64-bits
CentOS / 5.1 / 2.6.18-371.el5 / 32-bits
CentOS / 5.11 / 2.6.18-398.el5 / 64-bits
CentOS / 5.11 / 2.6.18-406.el5.centos.plus / 64-bits
CentOS / 5.2 / 2.6.18-92.el5 / 64-bits
CentOS / 5.4 / 2.6.18-164.el5 / 32-bits
CentOS / 5.4 / 2.6.18-164.el5 / 64-bits
CentOS / 5.4 / 2.6.18-164.el5PAE / 32-bits
CentOS / 5.4 / 2.6.18-308.el5 / 64-bits
CentOS / 5.4 / 2.6.32.el5 / 64-bits
CentOS / 5.4 / 2.6.32.el5 / 64-bits
CentOS / 5.4 / 2.6.32.el5 / 64-bits
CentOS / 5.4 / 2.6.37-6.el5.x86_64 / 64-bits
CentOS / 5.4 / 2.6.37.el5 / 64-bits
CentOS / 5.5 / 2.6.18-194.el5 / 64-bits
CentOS / 5.5 / 2.6.18-194.el5xen / 64-bits
CentOS / 5.5 / 2.6.32.el5 / 64-bits
CentOS / 5.5 / 2.6.37 / 64-bits
CentOS / 5.5 / 2.6.37-1 / 64-bits
CentOS / 5.5 / 2.6.37-2 / 64-bits
CentOS / 5.5 / 2.6.37-3 / 64-bits
CentOS / 5.5 / 2.6.37-4 / 64-bits
CentOS / 5.5 / 2.6.37-5 / 64-bits
CentOS / 5.5 / 2.6.37-6 / 64-bits
CentOS / 5.6 / 2.6.18-238.el5 / 64-bits
CentOS / 5.6 / 3.14.5-x86_64-linode42 / 64-bits
CentOS / 5.7 / 2.6.18-274.el5 / 64-bits
CentOS / 5.7 / 2.6.18-274.el5xen / 32-bits
CentOS / 5.7 / 2.6.18-274.el5xen / 64-bits
CentOS / 5.7 / 2.6.39-900.109.1.reiserfs.el5uek / 64-bits
CentOS / 5.8 / 2.6.18-308.el5 / 64-bits
CentOS / 5.8 / 2.6.18-308.el5xen / 64-bits
CentOS / 5.8 / 2.6.18-371.1.2.el5 / 64-bits
CentOS / 5.8 / 2.6.18-371.9.1.el5 / 64-bits
CentOS / 5.8 / 2.6.18-400.1.1.el5 / 64-bits
CentOS / 5.9 / 2.6.18-348.1.1.el5 / 64-bits
CentOS / 5.9 / 2.6.18-348.1.1.el5xen / 32-bits
CentOS / 5.9 / 2.6.18-348.18.1.el5xen / 64-bits
CentOS / 5.9 / 2.6.18-348.el5 / 64-bits
CentOS / 5.9 / 2.6.18-398.el5PAE / 32-bits
CentOS / 6.0 / 2.6.32-131.17.1.el6.x86_64 / 64-bits
CentOS / 6.0 / 2.6.32-71.el6.x86_64 / 64-bits
CentOS / 6.1 / 2.6.32-131.el6.x86_64 / 64-bits
CentOS / 6.10 / 2.6.32-754.el6.x86_64 / 64-bits
CentOS / 6.10 / 4.17.8-1.el6.elrepo.x86_64 / 64-bits
CentOS / 6.2 / 2.6.32-220.13.1.el6.x86_64 / 64-bits
CentOS / 6.2 / 2.6.32-220.2.1.el6.x86_64 / 64-bits
CentOS / 6.2 / 2.6.32-220.7.1.el6.x86_64 / 64-bits
CentOS / 6.2 / 2.6.32-220.el6.x86_64 / 64-bits
CentOS / 6.2 / 2.6.32-279.19.9.el6.ucloud.i686 / 32-bits
CentOS / 6.2 / 2.6.32-900.220.23.1.letv.el6.x86_64 / 64-bits
CentOS / 6.2 / 2.6.32-letv.2.220.4.1.el6.x86_64 / 64-bits
CentOS / 6.3 / 2.6.32-042stab065.3 / 64-bits
CentOS / 6.3 / 2.6.32-279.23.1.mi5.el6.x86_64 / 64-bits
CentOS / 6.3 / 2.6.32-279.el6.x86_64 / 64-bits
CentOS / 6.3 / 2.6.32-902.279.9.1.letv.el6.x86_64 / 64-bits
CentOS / 6.3 / 3.12.6-han / 64-bits
CentOS / 6.3 / 4.11.1-1.el6.elrepo.x86_64 / 64-bits
CentOS / 6.4 / 2.6.32-042stab072.10 / 64-bits
CentOS / 6.4 / 2.6.32-042stab106.4 / 64-bits
CentOS / 6.4 / 2.6.32-358.14.1.el6 / 64-bits
CentOS / 6.4 / 2.6.32-358.14.1.el6.x86_64 / 64-bits
CentOS / 6.4 / 2.6.32-358.18.1.el6.x86_64 / 64-bits
CentOS / 6.4 / 2.6.32-358.2.1.el6.x86_64 / 64-bits
CentOS / 6.4 / 2.6.32-358.23.2.el6.i686 / 32-bits
CentOS / 6.4 / 2.6.32-358.23.2.el6.x86_64 / 64-bits
CentOS / 6.4 / 2.6.32-358.el6.x86_64 / 64-bits
CentOS / 6.4 / 2.6.32-431.el6.i686 / 32-bits
CentOS / 6.4 / 2.6.32-431.el6.x86_64 / 64-bits
CentOS / 6.4 / 2.6.32-504.3.3.el6.x86_64 / 64-bits
CentOS / 6.4 / 2.6.32-903.279.9.1.letv.el6.x86_64 / 64-bits
CentOS / 6.4 / 2.6.32-925.431.23.3.letv.el6.x86_64 / 64-bits
CentOS / 6.4 / 3.12.el6 / 64-bits
CentOS / 6.5 / 2.6.32-042stab084.26 / 64-bits
CentOS / 6.5 / 2.6.32-042stab090.5 / 64-bits
CentOS / 6.5 / 2.6.32-042stab092.1 / 64-bits
CentOS / 6.5 / 2.6.32-279.19.8.el6.ucloud / 64-bits
CentOS / 6.5 / 2.6.32-431.11.15.el6.ucloud.x86_64 / 64-bits
CentOS / 6.5 / 2.6.32-431.11.25.el6.ucloud.x86_64 / 64-bits
CentOS / 6.5 / 2.6.32-431.11.5.el6.ucloud / 64-bits
CentOS / 6.5 / 2.6.32-431.20.3.el6.x86_64 / 64-bits
CentOS / 6.5 / 2.6.32-504.el6 / 64-bits3.11.47.1
CentOS / 6.5 / 2.6.32-504.el6.x86_64 / 64-bits
CentOS / 6.5 / 2.6.32-923.431.20.3.letv.el6.x86_64 / 64-bits
CentOS / 6.5 / 3.10.104-1.el6.elrepo.x86_64 / 64-bits
CentOS / 6.5 / 3.10.59 / 64-bits
CentOS / 6.5 / 3.12.6 / 64-bits
CentOS / 6.5 / 3.12.6-v1.3 / 64-bits
CentOS / 6.5 / 3.18.27.upyun / 64-bits
CentOS / 6.5 / 3.19.1-x86_64-linode53 / 64-bits
CentOS / 6.5 / 4.0.2-x86_64-linode56 / 64-bits
CentOS / 6.5 / 4.4.0-x86_64-linode63 / 64-bits
CentOS / 6.6 / 2.6.32-042stab108.8 / 64-bits
CentOS / 6.6 / 2.6.32-504.3.3.el6.centos.plus.x86_64 / 64-bits
CentOS / 6.6 / 2.6.32-504.3.3.el6.x86_64 / 64-bits
CentOS / 6.6 / 2.6.32-504.el6 / 32-bits
CentOS / 6.6 / 2.6.32-504.el6.i686 / 32-bits
CentOS / 6.6 / 2.6.32-573.1.1.el6.x86_64 / 64-bits
CentOS / 6.6 / 2.6.32-926.504.30.3.letv.el6.x86_64 / 64-bits
CentOS / 6.7 / 2.6.32-042stab112.15 / 64-bits
CentOS / 6.7 / 2.6.32-573.26.1.el6.x86_64 / 64-bits
CentOS / 6.7 / 2.6.32-696.el6.x86_64 / 64-bits
CentOS / 6.7 / 3.10.0-327.10.1.el6 / 64-bits
CentOS / 6.7 / 3.10.0-327.10.1.el6 / 64-bits
CentOS / 6.7 / 3.10.0-327.10.1.el6 / 64-bits
CentOS / 6.7 / 3.10.0-327.10.1.el6.r01_NG.x86_64 / 64-bits
CentOS / 6.7 / 3.12.6 / 64-bits
CentOS / 6.7 / 3.12.6-112 / 64-bits
CentOS / 6.7 / 4.17.14-1.el6.x86_64 / 64-bits
CentOS / 6.8 / 2.6.32-642.el6.x86_64 / 64-bits
CentOS / 6.8 / 3.10.105-1.el6.elrepo.x86_64 / 64-bits
CentOS / 6.8 / 3.12.6 / 64-bits
CentOS / 6.8 / 4.1.42-1.el6.x86_64 / 64-bits
CentOS / 6.8 / 4.17.11-1.el6.elrepo.x86_64 / 64-bits
CentOS / 6.8 / 4.4.170-1.el6.elrepo.x86_64 / 64-bits
CentOS / 6.8 / 4.9.7-1.el6.elrepo.x86_64 / 64-bits
CentOS / 6.9 / 2.6.32-696.1.1.el6.x86_64 / 64-bits
CentOS / 7 / 3.18.1-x86_64-linode50 / 64-bits
CentOS / 7 / 3.18.5-x86_64-linode52 / 64-bits
CentOS / 7.0 / 3.10.0-123.el7.x86_64 / 64-bits
CentOS / 7.0 / 3.10.0-862.3.3.el7.x86_64 / 64-bits
CentOS / 7.0 / 3.10.0-862.el7.x86_64 / 64-bits
CentOS / 7.0 / 4.9.6-1.el7.elrepo.x86_64 / 64-bits
CentOS / 7.0 / 4.9.7-1.el7.elrepo.x86_64 / 64-bits
CentOS / 7.1 / 3.10.0-229.1.2.el7.x86_64 / 64-bits
CentOS / 7.1 / 3.10.0-327.3.1.el7.x86_64 / 64-bits
CentOS / 7.1 / 3.10.75-2.el7.x86_64 / 64-bits
CentOS / 7.2 / 3.10.0-1-tlinux2_ntrace_cdn-0008.tl2 / 64-bits
CentOS / 7.2 / 3.10.0-327.el7.x86_64 / 64-bits
CentOS / 7.2 / 3.10.0-514.el7.x86_64 / 64-bits
CentOS / 7.2 / 3.10.104-1-tlinux2-0041.live.appex.tl2 / 64-bits
CentOS / 7.2 / 3.10.104-1-tlinux2-0041.live.appex2.tl2 / 64-bits
CentOS / 7.2 / 4.9.0-1.el7.elrepo.x86_64 / 64-bits
CentOS / 7.3 / 3.10.0-514.2.2.el7.x86_64 / 64-bits
CentOS / 7.4 / 3.10.0-693.1.1.el7.x86_64 / 64-bits
CentOS / 7.4 / 3.10.0-693.25.4.el7.x86_64 / 64-bits
CentOS / 7.4 / 4.11.2-1.el7.elrepo.x86_64 / 64-bits
CentOS / 7.4 / 4.20.12-1.el7.elrepo.x86_64 / 64-bits
CentOS / 7.6 / 3.10.0-957.el7.centos.plus.i686 / 32-bits
CentOS / 7.6 / 3.10.0-957.el7.x86_64 / 64-bits
CentOS / 7.6 / 4.20.11-1.el7.elrepo.x86_64 / 64-bits
CloudLinux_Server / 6.6 / 4.0.2-x86_64-linode56 / 64-bits
Debian / 6.0 / 3.2.0-0.bpo.4-amd64 / 64-bits
Debian / 7 / 3.14.5-x86_64-linode42 / 64-bits
Debian / 7 / 3.18.1-x86_64-linode50 / 64-bits
Debian / 7 / 3.18.5-x86_64-linode52 / 64-bits
Debian / 7 / 3.2.0-4-amd64 / 64-bits
Debian / 8 / 3.16.0-4-amd64 / 64-bits
Debian / 8 / 4.0.2-x86_64-linode56 / 64-bits
Debian / 8 / 4.4.10-1-pve / 64-bits
Debian / 9.3 / 4.9.0-4-amd64 / 64-bits
EulerOS / 2.0 / 3.10.0-862.14.0.1.h43.eulerosv2r7.x86_64 / 64-bits
Fedora / 12 / 2.6.31.5-127.fc12.i686.PAE / 32-bits
Gentoo / gentoo / 3.2.12-gentoo / 64-bits
Hikvision / 3.4.35 / Hikvision / 64-bits
neokylin / 3.2 / 2.6.32-279.5.ky3.1 / 32-bits
NewStart_CGS / 4 / 2.6.32-220.el6.x86_64 / 64-bits
NewStart_CGS_Linux_V4 / Released_By_ZTE / Kernel / 32-bits
Oracle / 6.2 / 2.6.39-200.24.1.el6uek.x86_64 / 64-bits
OWLinux / 4.0.3 / 2.6.26.8.1.OWLsmp / 64-bits
OWLinux / 4.2.1.2 / 2.6.32-220 / 64-bits
OWLinux / 4.2.1.2 / 3.4.13-3.1 / 64-bits
OWLinux / 4.2.1.2 / 3.4.13-3.1.OWLsmp / 64-bits
Poky / 1.6 / 3.10.34-ltsi-yocto-standard / 32-bits
Red_Hat_Enterprise / 5 / 2.6.18-53.el5 / 32-bits
Red_Hat_Enterprise / 5 / 2.6.18-53.el5 / 64-bits
Red_Hat_Enterprise / 5.2 / 2.6.18-92.el5 / 64-bits
Red_Hat_Enterprise / 5.4 / 2.6.18-164.el5 / 32-bits
Red_Hat_Enterprise / 5.4 / 2.6.18-164.el5 / 64-bits
Red_Hat_Enterprise / 5.4 / 2.6.18-164.el5PAE / 32-bits
Red_Hat_Enterprise / 5.4 / 2.6.32.el5 / 64-bits
Red_Hat_Enterprise / 5.5 / 2.6.18-194.el5 / 64-bits
Red_Hat_Enterprise / 5.5 / 2.6.18-194.el5xen / 64-bits
Red_Hat_Enterprise / 5.6 / 2.6.18-238.el5 / 64-bits
Red_Hat_Enterprise / 5.7 / 2.6.18-274.el5 / 64-bits
Red_Hat_Enterprise / 5.7 / 2.6.18-274.el5xen / 32-bits
Red_Hat_Enterprise / 5.7 / 2.6.18-274.el5xen / 64-bits
Red_Hat_Enterprise / 5.8 / 2.6.18-308.el5 / 64-bits
Red_Hat_Enterprise / 5.8 / 2.6.18-308.el5xen / 64-bits
Red_Hat_Enterprise / 6 / 2.6.32-56 / 64-bits
Red_Hat_Enterprise / 6.0 / 2.6.32-71.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.1 / 2.6.32-131.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.1 / 2.6.32-220.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.2 / 2.6.32-2.0.0.1.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.2 / 2.6.32-2.0.0.8.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.2 / 2.6.32-220.23.1.tb1.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.3 / 2.6.32-276.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.3 / 2.6.32-279.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.4 / 2.6.32-358.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.4 / 2.6.32-431.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.4 / 2.6.39-400.17.1.el6uek.x86_64 / 64-bits
Red_Hat_Enterprise / 6.5 / 2.6.32-431.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.6 / 2.6.32-504.3.3.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.6 / 2.6.32-504.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 6.6 / 2.6.32-573.1.1.el6.x86_64 / 64-bits
Red_Hat_Enterprise / 7.0 / 3.10.0-123.el7.x86_64 / 64-bits
Red_Hat_Enterprise / 7.0 / 4.9.6-1.el7.elrepo.x86_64 / 64-bits
Red_Hat_Enterprise / 7.1 / 3.10.0-229.1.2.el7.x86_64 / 64-bits
Red_Hat_Enterprise / 7.2 / 3.10.0-327.el7.x86_64 / 64-bits
Red_Hat_Enterprise / 7.2 / 3.10.0-514.el7.x86_64 / 64-bits
Red_Hat_Enterprise / 7.3 / 3.10.0-514.6.1.el7.x86_64 / 64-bits
Red_Hat_Enterprise / 7.4 / 3.10.0-693.1.1.el7.x86_64 / 64-bits
Red_Hat_Enterprise / 7.4 / 3.10.0-693.17.1.el7.x86_64 / 64-bits
Red_Hat_Enterprise / 7.6 / 3.10.0-957.el7.x86_64 / 64-bits
Surfos / 6.2 / 3.8.4 / 64-bits
SUSE_Linux_Enterprise / 11 / 2.6.32.12-0.7-default / 64-bits
SUSE_Linux_Enterprise / 11 / 2.6.32.59-0.7-default / 64-bits
SUSE_Linux_Enterprise / 11 / 3.0.101-0.47.105.1.13184.1.PTF-default / 64-bits
SUSE_Linux_Enterprise / 11 / 3.0.13-0.27-default / 64-bits
SUSE_Linux_Enterprise / 11 / 3.0.76-0.11-default / 64-bits
SUSE_Linux_Enterprise / 11.4 / 3.0.101-63-default / 64-bits
Tencent_tlinux / 2.0 / 3.10.0-1-tlinux2_cdn_nosign-0001.tl2 / 64-bits
Tencent_tlinux / 2.0 / 3.10.0-1-tlinux2_ntrace_cdn-0001.tl2 / 64-bits
Tencent_tlinux / 2.0 / 3.10.104-1-tlinux2-0041.live.appex.0809.tl2 / 64-bits
Tencent_tlinux / 2.0 / 3.10.104-1-tlinux2-0041.live.appex.tl2 / 64-bits
Tencent_tlinux / 2.0 / 3.10.104-1-tlinux2-0041.live.appex2.tl2 / 64-bits
Tencent_tlinux / 2.0 / 3.10.104-1-tlinux2-0041.live.appex3.tl2 / 64-bits
Ubuntu / 10.04.4 / 2.6.32-38-generic-pae / 32-bits
Ubuntu / 11.10 / 3.0.0-12-server / 64-bits
Ubuntu / 11.10 / 3.0.0-14-virtual / 64-bits
Ubuntu / 12.04 / 3.2.0-23-generic / 64-bits
Ubuntu / 12.04 / 3.2.0-24-virtual / 32-bits
Ubuntu / 12.04 / 3.2.0-4-686-pae / 32-bits
Ubuntu / 12.04 / 3.2.0-56-virtual / 64-bits
Ubuntu / 12.04 / 3.2.0-59-generic / 64-bits
Ubuntu / 12.04 / 3.2.0-60-generic / 64-bits
Ubuntu / 12.04 / 3.2.0-61-generic / 64-bits
Ubuntu / 12.04 / 3.2.0-70-generic / 64-bits
Ubuntu / 12.04 / 3.5.0-23-generic / 64-bits
Ubuntu / 12.04 / 3.5.0-23-generic / 32-bits
Ubuntu / 12.04 / 3.5.0-45-generic / 64-bits
Ubuntu / 12.04 / 3.5.0-54-generic / 64-bits
Ubuntu / 12.04 / 3.8.0-35-generic / 64-bits
Ubuntu / 12.04 / 3.8.0-44-generic / 64-bits
Ubuntu / 12.04 / 4.0.2-x86_64-linode56 / 64-bits
Ubuntu / 12.04.1 3.2.0-31-generic / 64-bits
Ubuntu / 12.04.2 3.2.0-40-generic / 64-bits
Ubuntu / 12.04.5 3.2.0-106-generic / 64-bits
Ubuntu / 13.10 / 4.9.0-040900rc8-generic 64-bits
Ubuntu / 14.04 / 3.13.0-117-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-24-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-24-generic / 32-bits
Ubuntu / 14.04 / 3.13.0-29-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-29-generic / 32-bits
Ubuntu / 14.04 / 3.13.0-32-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-36-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-37-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-40-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-43-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-44-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-45-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-46-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-48-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-55-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-74-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-79-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-83-generic / 64-bits
Ubuntu / 14.04 / 3.13.0-85-generic / 64-bits
Ubuntu / 14.04 / 3.16.0-28-generic / 64-bits
Ubuntu / 14.04 / 3.16.0-30-generic / 64-bits
Ubuntu / 14.04 / 3.16.0-38-generic / 64-bits
Ubuntu / 14.04 / 3.16.0-43-generic / 64-bits
Ubuntu / 14.04 / 3.16.5-linode46 / 64-bits
Ubuntu / 14.04 / 3.16.5-linode65 / 32-bits
Ubuntu / 14.04 / 3.18.1-x86_64-linode50 / 64-bits
Ubuntu / 14.04 / 3.18.5-x86_64-linode52 / 64-bits
Ubuntu / 14.04 / 3.19.0-25-generic / 64-bits
Ubuntu / 14.04 / 3.19.0-80-generic / 64-bits
Ubuntu / 14.04 / 3.8.13-generic / / 32-bits
Ubuntu / 14.04 / 4.2.0-35-generic / 64-bits
Ubuntu / 14.04 / 4.4.0-38-generic / 64-bits
Ubuntu / 14.04.4 3.13.0-147-generic / 64-bits
Ubuntu / 14.04.4 3.13.0-92-generic / 64-bits
Ubuntu / 14.04.5 3.16.0-77-generic / 64-bits
Ubuntu / 15.10 / 4.2.0-16-generic-imq / 64-bits
Ubuntu / 15.10 / 4.2.8-ckt8 / / 64-bits
Ubuntu / 16.04 / 4.4.0-142-generic / 64-bits
Ubuntu / 16.04 / 4.4.0-47-generic / 64-bits
Ubuntu / 16.04 / 4.8.0-36-generic / 64-bits
Ubuntu / 18.04 / 4.15.0-30-generic / 64-bits
Alibaba_Group_Enterprise_Linux_Server / 6.2 / 2.6.32-220.1.alios6.x86_64 / 64-bits