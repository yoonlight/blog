# Linux

* set static ip
  * <https://linuxconfig.org/how-to-configure-static-ip-address-on-ubuntu-18-10-cosmic-cuttlefish-linux>
* zip
  * <https://linuxize.com/post/how-to-create-and-extract-archives-using-the-tar-command-in-linux/>
* iptables
  * allow port

  ```shell
  iptables -I INPUT -p tcp -m tcp --dport 80 -j ACCEPT
  ```

  * save iptables rule

  ```shell
  sudo service iptables save
  ```

  * <https://docs.rackspace.com/support/how-to/allow-web-traffic-in-iptables/>
* Version check
  * CentOS
    ```shell
    cat /etc/redhat-release
    ```
* APT mirror chaange
  ```shell
  sudo sed -i 's/kr.archive.ubuntu.com/mirror.kakao.com/g' /etc/apt/sources.list
  ```
* change hostname
  ```shell
  sudo vi /etc/hostname
  sudo vi /etc/hosts
  sudo reboot
  ```
  * <https://www.cyberciti.biz/faq/ubuntu-change-hostname-command/>
