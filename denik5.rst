denik 5
=======

`Zpet na obsah <https://bravo-cizek.github.io/>`_

Dnes jsem se naucil pripojit se k wifi a prizpusobit si rozliseni.
------------------------------------------------------------------

1. WiFi
-------

- v /etc/wpa_supplicant, vytvorit wpa_supplicant.conf
- do wpa_supplicant.conf ::

        ctrl_interface=/run/wpa_supplicant
        ctrl_interface_group=wheel
        eapol_version=1
        ap_scan=1
        fast_rauth=1
        update_config=1

        # Add here your networks.
        netwok={
          ssid="jmeno site"
          psk="heslo"
          }
                           
- pokud se nechce pripojit, da se vyuzit prikaz > ``sudo wpa_supplicant -B -i wlp00s0 -c /etc/wpa_supplicant/wpa_supplicant.conf``
- wlp00s0 = jmeno site, da se zjistit pomoci > ``ip a``


2. Rozliseni
------------

- Pro trvale ulozeni rozliseni > ``vim ~/.xinitrc``
- staci zapsat dve radky kodu ::
  
        xrandr -q
        xrandr --output "nazev vystupu" --mode rozliseni (1600x900)

- Poznamka, ``xrandr -q`` je tam z duvodu toho, ze bez nej, to z nejakeho duvodu nefunguje.
