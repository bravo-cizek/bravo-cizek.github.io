denik 7
=======

Git config
----------

- Tak samozrejme prvnim krokem je, instalace gitu. Nasleduje config user nameu a user emailu ::


                git config --global user.name "jmeno"
                git config --global user.email "email"

- Dalsim krokem je nastaveni ssh, nejdrive se muzu podivat jestli nejaky uz neexistuje v ``~/.ssh/``
- Pokud neexistuje, tak si ho musime vyrobit ``ssh-keygen -t rsa -C "muj_email@priklad.com``
- Nyni si samozrejme musim ten klic zkopirovat na svuj github.
- pro tuto prilezitost jsem vyuzil ``xclip``, jelikoz mi nefungovalo vlozeni pomoci leveho a praveho tlacitka ::

        xclip -sel clip < ~/.ssh/id_rsa.pub

- nasledovalo vlozeni ssh klice na muj github

- pro test spojeni jsem vyuzil ``ssh -T git@github.com`` vyhodilo mi to varovani, ale po procteni manualu z (https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/testing-your-ssh-connection), jsem zjistil ze je vse v poradku.

- nasledovalo ``git init`` pro vytovreni prazdneho git repa.
- a zkopirovani configu od romana z (https://github.com/roman-neuhauser/dotfiles-git)
 
