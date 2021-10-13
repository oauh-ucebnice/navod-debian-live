# Spuštění Live DVD Debianu ve VirtualBoxu na OA

> Umístění souborů je určeno pro Obchodní akademii Uherské Hradiště, zbytek návodu ale bude fungovat kdekoliv.

1. Spusť VirtualBox a&nbsp;vytvořte nový virtuální stroj<br />![](deb-live_010_virtualbox-new.png)
1. Přepni dialog do „expertního režimu“<br />![](deb-live_020_virtualbox-expertni.png)
1. Nepřidávej virtuální disk — Live DVD bude startovat z&nbsp;DVD<br />![](deb-live_030_nastaveni-vm.png)
1. Do virtuální DVD mechaniky musíme vložit Live DVD<br />![](deb-live_040_nastaveni.png)
1. Vyber soubor s&nbsp;Live DVD z&nbsp;disku D:<br />![](deb-live_050_cd.png)
<br />![](deb-live_060_iso.png)
1. Pokud na disku D: soubor není, zkopíruj si ho ze serveru `\\Dilna`<br />
Doma můžeš Live DVD stáhnout ze stránek: [https://www.debian.org/CD/live/](https://www.debian.org/CD/live/)<br />
![](deb-live_070_copy-iso-dilna.png)
1. Potvrď nastavení<br />![](deb-live_080_ok.png)
1. Spusť stroj<br />![](deb-live_090_spustit.png)
1. Potvrď spuštění Live DVD<br />![](deb-live_100_grub.png)
1. Uživatelský účet je `user`, `sudo` lze provádět bez hesla<br />![](deb-live_110_sudo.png)
1. Stroj vypneš příkazem `sudo systemctl poweroff`<br />![](deb-live_120_poweroff.png)
1. DVD není třeba vytahovat (příště budeme opět používat Live DVD), stačí zmáčknout Enter<br />![](deb-live_130_enter.png)
