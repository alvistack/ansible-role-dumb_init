# Ansible Role for dumb-init

## 4.2.7 - 2020-04-01

### Major Changes

  - [DEPRECATED] Sync with `docker --init`, use tini instead
  - Upgrade minimal Molecule support to 3.0.2
  - Migrate role name to lowercase or underline
  - Migrate group name to lowercase or underline
  - Migrate molecule `group_vars` to file
  - Consolidate molecule tests into `default` (noop)
  - Download archives to `{{ ansible_user_dir }}/.ansible/tmp`

## 4.2.0 - 2020-02-13

### Major Changes

  - Migrate molecule driver to Libvirt
  - Migrate molecule verifier to Ansible
  - Support Ubuntu 19.10

## 4.1.0 - 2020-01-16

### Major Changes

  - Default `interpreter_python` with `python3`
  - Bugfix `python3-xml` not exists for openSUSE Leap 15.1

## 4.0.0 - 2019-11-05

### Major Changes

  - Upgrade minimal Ansible support to 2.9.0
  - Upgrade Travis CI test as Ubuntu Bionic based

## 3.5.0 - 2019-10-06

### Major Changes

  - Support openSUSE Leap 15.1
  - Default with Python 3
  - Revamp molecule test with vagrant

## 3.4.0 - 2019-09-18

### Major Changes

  - Run molecule test manually on Travis CI

## 3.3.0 - 2019-08-27

### Major Changes

  - Update for RHEL 7
  - Add Vagrant test for RHEL 7
  - Download archives to `/var/cache/ansible`
  - Upgrade packages if archives not found from `/var/cache/ansible`

## 3.2.0 - 2019-07-08

### Major Changes

  - Update LXD test profile for Kubernetes v1.15.0 support
  - Add dummy tasks and vars placeholder for multi OS support
  - Fix molecule `group_vars` with links
  - Replace `with_items` with `loop`
  - Replace `with_dict` with `var`
  - Replace `with_first_found` with `lookup('first_found')`

## 3.1.0 - 2019-06-13

### Major Changes

  - Always include default variables from `vars/main.yml`
  - Always use `become: true` with molecule, especially for vagrant
  - Abstract archive download checksum with multiple version support

## 3.0.0 - 2019-05-20

### Major Changes

  - Upgrade minimal Ansible support to 2.8.0

## 2.6.0 - 2019-05-04

### Major Changes

  - Refine Travis CI Molecue test cases

## 2.5.0 - 2019-04-17

### Major Changes

  - Pre-download archives with checksum
  - Run test with `travis_wait 120`

## 2.4.0 - 2019-03-03

### Major Changes

  - Rollback to direct download binary, skip python dependency
  - Add openSUSE Leap 15 support
  - Remove CentOS 6 support

## 2.3.0 - 2019-01-30

### Major Changes

  - Porting test to Molecule based

## 2.2.0 - 2019-01-25

  - Minor typo fix

## 2.1.0 - 2018-12-06

### Major Changes

  - CI with yamllint, ansible-lint and ansible-playbook --syntax-check
  - CI with LXD, improve systemd support
  - Use shell only when shell functionality is required
  - Install dumb-init from PIP, simplify upgrade path

## 2.0.0 - 2018-10-25

### Major Changes

  - Upgrade Ansible support to 2.6 or higher
  - Support both Ubuntu 16.04/18.04 and RHEL/CentOS 6/7
  - Upgrade dumb-init to v1.2.2
  - Update Travis CI test plan

## 1.1.0 - 2017-11-23

### Major Changes

  - Install dumb-init on Ubuntu 16.04/14.04 and CentOS 7/6 from source
  - Update test cases

## 1.0.0 - 2017-09-25

  - Ininitial release for Ansible 2.4
  - Support both Ubuntu 16.04/14.04 or RHEL/CentOS 7/6
