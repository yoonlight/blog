# Linux

## Command

### Tar
* Ref
  * <https://linuxize.com/post/how-to-create-and-extract-archives-using-the-tar-command-in-linux/>

### iptables
* Command
  * allow

  ```shell
  iptables -I INPUT -p tcp -m tcp --dport 80 -j ACCEPT
  ```

  * save iptables rule

  ```shell
  sudo service iptables save
  ```

* Ref
  * <https://docs.rackspace.com/support/how-to/allow-web-traffic-in-iptables/>

### Version check 
* CentOS
  ```shell
  cat /etc/redhat-release
  ```
