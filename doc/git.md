# SSH key, GitHub and git configuration

1. Create SSH key

    ```bash
    $ ls ~/.ssh
    $ ssh-keygen -t rsa -b 4096 -C "<your_email>"
    $ cat ~/.ssh/id_rsa.pub
    ```

2. Add SSH key to your GitHub. [GitHub config page](https://github.com/settings/keys)

3. GitHub connection test.

    ```bash
    $ ssh -T git@github.com
    ```

4. git config

    ```bash
    $ git config --global user.name <your_name>
    $ git config --global user.email <your_email>
    $ git config --global core.editor vim
    $ git config --global push.default matching
    $ git config --global core.quotepath false
    ```

