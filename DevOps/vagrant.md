# Vagrant
 
* IaC, Infrastructure as Code
* Provisioning
  * [Provisioning is the process of setting up IT infrastructure.](https://www.redhat.com/en/topics/automation/what-is-provisioning)
* Command
  * generate vagrant file
  ```shell
  vagrant init
  ```
  * vagrant file start
  ```shell
  vagrant up
  ```
  * access vm through ssh
  ```shell
  vagrant ssh
  ```
  * Delete Provisioning VM
  ```shell
  vagrant destroy -f
  ```
  * Change VM Setting
  ```shell
  vagrant provision
  ```

## Hyper-V
* <https://docs.microsoft.com/en-us/virtualization/community/team-blog/2017/20170706-vagrant-and-hyper-v-tips-and-tricks#tip-0-install-hyper-v>

## Ref.

* [Test infrastructure](https://thebook.io/080241/ch02/)
* [Command](https://thebook.io/080241/ch02/01/03/)
* [Vagrant Image](https://app.vagrantup.com/boxes/search)
* [Creating a Base Box](https://www.vagrantup.com/docs/boxes/base)
* Example
  * [Single Machine Code](https://thebook.io/080241/ch02/02/01-01/)
  * [Multi Machine Code](https://thebook.io/080241/ch02/02/03-01/)
