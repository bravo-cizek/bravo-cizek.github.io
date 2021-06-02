denik 4
=======

`Zpet na obsah <https://bravo-cizek.github.io/>`_

opakovani instalace programu a jejich nasledny config
---------------------------------------------------------

- instalace programu pomoci xbps-install
- config souboru, zatim mi staci stahnout si configy od romana z githubu
- nasledne je dulezite tyhle soubory rozkopirovat na spravna mista!! ::

    for x in vim i3 zsh xorg; do
      git clone https://github.com/roman-neuhauser/dotfiles-$x
      cp -rp dotfiles-$x/.* ~/
    done


config i3 window manageru
---------------------------

- zatim staci zkopirovat config od romana z ``https://github.com/roman-neuhauser/dotfiles-i3``
- nasledne ho ulozit do ``~/.config/i3/config``
- smaozrejme si ho muzu prizpusobit sam, staci si ve vimu otevrit config ``vim ~/.config/i3/config`` 
- potom uz jen prepisovani podle manualu
