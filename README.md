# Školní-projekt

# 1. Cíl projektu
Mým cílem tohoto projektu bylo sebezdokonalení a doučení v oblasti sítí. Samotným cílem projektu bylo vytvoření sítě v budově, která má tři poschodí.

# 2. Stav projektu 
Veškerý popis je níže, kde najdete veškerou konfiguraci a ostatní. Každé zařízení má svou adresu a je přiděleno do příslušný VLAN.
Je zde také nastavený DHCP server a pro komunikaci na dálku je použita šifrovaná komunikace přes SSH. Každé poschodí má také AP-PT pro Wi-Fi.
Tento projekt je dle mě hotový. Pro otevření mého projektu musíte stáhnout Packet Tracer.
+popis je upraven ai !! CÉLÝ TEXT JE VYTVOŘEN MNOU A MÝMI SLOVY JEDINÉ DOPOMOC OD AI BYLA OPRAVA PRAVOPISNÝCH CHYB ABY TO BYLO LÉPE ČITELNÉ !!

# 3. Popis projektu
Zde je obrázek mého projektu:
<img width="1247" alt="vis1" src="https://github.com/user-attachments/assets/7f83336a-caf3-4a31-9a5c-fff79bd57217" />

## Popis:
### Zařízení a propojení:
Jsou zde 3 poschodí. V každém poschodí je jeden router a jeden switch, plus v jedné místnosti je AP. Každé poschodí se skládá ze tří místností, kromě třetího, kde jsou jen 2 místnosti. Každá místnost má alespoň dvě koncová zařízení, například PC a tiskárnu, a svou vlastní adresu se svým Virtuálním LAN.

Všechny routery jsou propojeny DCE kabelem, který má červenou barvu a často se používá mezi routery pro synchronizovanou datovou komunikaci. Zbylá zařízení jsou propojena klasickým měděným přímým kabelem označeným černou barvou. Dodatečná zařízení jsou připojena vzdáleně přes AP. To by bylo propojení a vysvětlení zařízení.
                              
### Aresace a Virtuální LAN: 
Nejdříve začnu adresami a VLAN. Adresy mezi routery jsou 10.10.10.8/30. Tato IP adresa, na rozdíl od klasických lokálních, je zde, aby se vyhnula kolizím, a maska /30 je použita, protože chceme mít co nejméně volných adres kvůli bezpečnosti a jednoduchému správování adres. Pak zde máme klasické lokální adresy začínající 192.168.x.x/24, které jsou běžné v lokálních sítích, a maska /24 je použita pro dodatečné rozšíření. VLAN, neboli Virtual Local Area Network, slouží k oddělení sítí, usnadňuje provoz v síti a zajišťuje zabezpečení.
### Obrázek ke konfiguraci a funkcím
<img width="1912" alt="Vis4" src="https://github.com/user-attachments/assets/e706892c-5d9e-4c77-bf88-e027f2849606" />

### Konfigurace a funkce:
VLAN port mezi switchem a routerem, který je fyzicky připojený, je nastavený na mód trunk. Ten je zde pro komunikaci, aby byla správná segmentace, neboli říká, jaký VLAN je jaký. Pak zde jsou nastaveny samotné VLAN, takže určité porty jsou aktivovány. VLAN se rozlišují čísly.

DHCP, neboli Dynamic Host Configuration Protocol, jak název napovídá, je protokol, který automaticky přiděluje adresy. Výhoda tohoto protokolu je šetření adres a zabránění nechtěným kolizím mezi adresami. Velmi se hodí, protože je jednodušší dostat adresu než si ji manuálně přidělovat.

DNS, neboli Domain Name System, je také protokol a jeho funkce je překlad domény na IP adresu. Zde je využit pro funkci DHCP serveru, neboť bez něj nefunguje.

Pak zde máme počítač admina, který je zabezpečen tak, že v síti může být jen jeho zařízení s tiskárnou. Je to zde jen pro bezpečnost.

SSH, neboli Secure Shell, je zde pro komunikaci z PC mezi ostatními zařízeními. Funkcí je velmi podobný komunikaci přes Telnet, ale jeho výhodou je bezpečnost. Telnet je nešifrovaný, zatímco pro SSH se vytvoří šifrovací klíče, takže komunikace přes SSH je bezpečná a nejde odposlouchávat. Komunikace je ještě zabezpečená heslem.

Teď se dostáváme k využití AP. Je to krabička, která umožňuje bezdrátové dodatečné připojení. Je zde nastavené SSID a heslo pro ochranu. Zařízení, která mají možnost připojení k bezdrátové síti, se mohou připojit a komunikovat. Adresa je dána automaticky, protože je zde DHCP.

Pokud máte další otázky nebo potřebujete více informací, dejte mi vědět!
### Závěr:
Toto bylo moje vysvětlení pokud by byly nějaké nejasnosti tak mi napište nebo mi řekněte ve škole cokoli co nebudete chápat tak vám klidně vysvětlím vím že jste mi doporučil udělat video jenomže můj problém je že toto témá je trochu koplikované a mám prostě problémy se vyjadřovat takže za to se omlouvám ale do příště to určitě napravím a video udělám SLIBUJU  

# 4. Členi 
Pracoval jsem sám a veškeré zdroje jsou uvedeny níže.

# 5. Citace
[1] Cisco. Online. S. 1. Dostupné z: https://www.cisco.com/#tabs-35d568e0ff-item-194f491212-tab. [cit. 2025-01-06].

[2] Cisco. Online. S. 1. Dostupné z: https://www.cisco.com/c/en/us/solutions/small-business/resource-center/networking/how-to-setup-network-switch.html. [cit. 2025-01-06].

[3] Gurutech Networking Training. Online. Dostupné z: https://www.youtube.com/@gurutechnetworks. [cit. 2025-01-06].

# 6. Zdroje
 Při vytváření tohoto projektu jsem vytvořil dva pod projetky ze kterých jsem dále vycházel. 
 
 Zdroje:
 
 https://www.cisco.com/#tabs-35d568e0ff-item-194f491212-tab   
 https://www.cisco.com/c/en/us/solutions/small-business/resource-center/networking/how-to-setup-network-switch.html
 https://www.cisco.com/c/en/us/td/docs/routers/access/800M/software/800MSCG/routconf.html
 https://www.youtube.com/@gurutechnetworks 


