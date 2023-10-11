# Instalace Debianu na virtuální stroj

## Stažení obrazu ve škole

Stažení obrazu ve škole (použijte **aktuální verzi**):
1. <br />![](img/010_dilna.png)
1. <br />![](img/020_d-img.png)

Stažení obrazu doma:
1. Pokud stahujete obraz doma, použijte stažení varianty <code>netinst</code> (síťová instalace, malé instalační médium) ze stránek [Debian.org](https://www.debian.org):<br />![](img/030_download.png)

## Vytvoření virtuálního stroje
1. Vytvořte nový virtuální stroj ve VirtualBoxu:<br />![VirtualBox: nastavení stroje](img/040_vm-config.png)
1. <br />![](img/045_vm-config-cpu.png)
1. <br />![](img/050_vm-disk.png)
1. <br />![](img/060_start.png)
<!---1. <br />![](img/070_select-dvd.png)
1. <br />![](img/080_add-iso.png)-->

## Postup instalace
1. <br />![](img/090_installer.png)
1. <br />![](img/100_lang.png)
1. <br />![](img/110_lang2.png)
1. <br />![](img/120_keyb.png)
1. <br />![](img/125_install.png)
1. Název počítače se zobrazí v&nbsp;příkazovém řádku<br />
_Doma si nastavte, co chcete. Ve škole, prosím, dodržte uvedený vzor. Když školní správce sleduje spuštěné počítače, vidí, že se jedná o virtuální stroj._<br />![Ve škole dodržte název počítače podle vzoru.](img/130_hostname.png)
1. <br />![](img/140_domain.png)
1. Přečtěte si důkladně popis! Nezadávejte žádné heslo pro uživatele `root`. Užiavtelský účet `root` tak bude zablokován a instalátor se vás následně zeptá na běžný uživatelský účet, kterému nastaví možnost použít příkaz `sudo`. To je doporučený postup (_best practice_).<br />![Nezadávejte heslo uživatele root! (Viz popis na obrazovce.)](img/150_no-root.png)
1. Zadejte plné jméno vašeho uživatelského účtu. Je celkem jedno, co zadáte.<br />![Plné jméno uživatele se uloží, ale skoro nikde se nepoužívá. ;)](img/160_username.png)
1. Zde zadejte váš login. Je to vaše osobní nastavení, vyberte si, jaký chcete. Ale nezapomeňte ho!<br />![Zadejte svůj login.](img/170_username2.png)
1. Doporučujeme silné heslo, aby si spolužáci nemohli omylem spustit váš stroj. Ale je to na vás.<br />![Doporučujeme silné heslo.](img/180_passwd.png)
1. <br />![](img/190_rozdeleni.png)
1. <br />![](img/200_disk.png)
1. Pro základní výuku práce v CLI stačí jednoduché rozdělení s&nbsp;jednou oblastí.<br />
_Doma můžete experimentovat i s&nbsp;dalšími rozděleními disku. Na funkci stroje to příliš nemění. Má to smysl u produkčních serverů, kde zaplnění například adresáře `/var` nebo `/home` neohrozí funkci zbytku systému._<br />![](img/210_vse-v-jednom.png)
1. <br />![](img/220_format.png)
1. <br />![](img/230_format.png)
1. <br />![](img/240_copy.png)
1. <br />![](img/250_dalsi-ne.png)
1. <br />![](img/250_mirror.png)
1. <br />![](img/260_mirror2.png)
1. <br />![](img/270_no-proxy.png)
1. <br />![](img/280_apt.png)
1. <br />![](img/290_baliky.png)
1. Nyní se instalátor ptá, jaké součásti chcete nainstalovat.<br />
_Ve škole neinstalujte grafické uživatelské rozhraní &mdash; zbytečně tím zabíráte místo na disku. Navíc se chceme učit pracovat na serveru, kde také GUI nejspíš nebude. Klidně si ale vytvořte doma další virtuální stroje a experimentujte!_<br />![](img/300_tasksel.png)
1. <br />![](img/310_install.png)
1. GRUB umožňuje při spuštění počítače vybrat správný operační systém a spustit ho. I když máte na virtuálním stroji jen Linux, GRUB nainstalovat potřebujete.<br />![](img/320_grub.png)
1. <br />![](img/330_grub2.png)
1. <br />![](img/340_hotovo.png)

## První spuštění a vypnutí
1. Nyní můžete nastartovat svůj nově nainstalovaný stroj:<br />![](img/350_boot.png)
1. Přihlaste se uživatelským jménem a heslem, které jste si nastavili:<br />![](img/360_login.png)
1. Můžete zkoušet práci s&nbsp;příkazy:<br />![](img/370_cli.png)
1. Až skončíte, vypněte systém řádně příkazem!<br />
_Pokud byste prostě jen zavřeli okno VirtualBoxu, je to obdoba vytažení běžícího počítače ze zásuvky. Sice se někdy nemusí stát nic, ale může také dojít k&nbsp;poškození nainstalovaného operačního systému. Sice je to jen virtuální stroj, ale instalovat znovu se vám ho asi nechce... ;)_<br />![](img/380_shutdown.png)


