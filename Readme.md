#Install Something For New Macbook Pro
- Reinstall Homebrew to solve one error 
(Error: An exception occurred within a child process:
	Errno::EACCES: Permission denied @ dir_s_mkdir - /usr/local/var/lib/rabbitmq)

```text
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/uninstall)"
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

- Install Rabbitmq
```text
brew update
brew install rabbitmq
```

- Add New User
/usr/local/sbin/rabbitmqctl list_users
/usr/local/sbin/rabbitmqctl add_user abcdefg abpassword

- Set Permission on local web page
http://127.0.0.1:15672/#/users
set permission

- Virtual Env Create
```text
sudo pip3 install virtualenv
virtualenv --python=python3 venv_pure3
```

