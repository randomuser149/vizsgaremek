# Leírás
A technikusi vizsgára csapatmunkában készített vizsgaremek dokumentációja.  
A feladat 2-3 fős csapatokat alkotva egy elképzelt vagy valós cég hálózatának tervezését, a hálózat  
egy működő prototípusának gyakorlati kivitelezését, valamint a prototípus működésének tesztelését foglalja magában.  
Követelmények (részlet):  
Legalább 3 telephelyet lefedő hálózati infrastruktúra  
VLAN-ok, IPv4/IPv6, statikus és dinamikus routing/NAT  
VPN, ACL-ek, hardveres tűzfal  
Linux és Windows szerverek (AD, DHCP, DNS, HTTP/HTTPS, fájlmegosztás, mentés, szoftvertelepítés)  
Dokumentáció, tesztelési jegyzőkönyv, 2–5 perces bemutató videó  
Szóbeli előadás magyarul valamint 2-3 perces angol részlet.  
a feladat pontos kiírása megtalálható az alábbi [https://api.ikk.hu/v1/media/documents/9215?filename=Informatikai-rendszer-%C3%A9s-alkalmaz%C3%A1s-%C3%BCzemeltet%C5%91-technikus-2023.11.21.-v3.pdf](linken)  

# Vizsgaremek
Anycompany cég hálózatát terveztük és alakítottuk ki, figyelve a következetes, egyértelmű, könnyen bővíthető és skálázható kialakításra egy közepes/nagyvállalat igényeinek megfelelően. Több eszköz használatával valósítottuk meg a prototípust: Packet Tracer-ben konfiguráltuk a hálózatot, VMware-ben futtatuk a szervereket, amiket egy egyszerűsített GNS 3 hálózatba integráltunk hogy szimulálni tudjuk a teljes szolgáltatási láncot valós szerverekkel. Munkánkat folyamatosan dokumentáltuk és alaposan teszteltük.  
Mivel a GitHub nem támogatja a .pdf, .docx és .xlsx fájlokat ezért ezek egy nyilvánosan megosztott Google Drive mappában találhatók az alábbi [](linken).

# Csapatmunka
A kivitelezést, konfigurálást és dokumentálást az alábbi módon osztottuk fel:
Dokumentum | Fődi Mátyás | Balogh Barnabás | Patkós Ádám | Megjegyzés
-----------|------------|-----------------|------------|-------
Vizsgaremek dokumentáció.pdf | 9-33 Bordeaux; 57-60 ISP; 61-74 Szerverek | 44-52 Budapest  | 34-43 Copenhagen; 53-56 Székesfehérvár | A feladat dokumentálása, a "mit és miért"
vizsgaremek.mp4 | Tesztelési anyagok | Tesztelési anyagok | Tesztelési anyagok & videó megvágása  | A hálózat és szerverek működésének tesztelése egy 5 perces videóba tömörítve
Bordeaux ACL.xlsx<br>"ordeaux HSRP.pdf<br>Bordeaux VLANs.pdf<br>IP Table Bordeaux.xlsx | egész | - | - | Bourdeaux részletes ACL, HSRP, VLAN és IP táblázat dokumentációja 
ISP DNS settings.pdf | egész | - | - | Az ISP DNS kialakításának leírása
IP Table Cphg Bp.xlsx | - | Budapest | Copenhagen | Budapest és Copenhagen IP táblája
IP Table ISP.pdf | egész | - | - | ISP IP táblája
IP Table Székesfehérvár.pdf | - | - | egész | Székesfehérvár IP táblája
autobackup.py<br>backup.py<br>backupall.py<br>conn_template.py<br>hsrp.py<br>interfaces.py<br>setBanner.py<br>setLogging.py<br>setNTP.py<br> | egész | - | - | Python fájlok Netmiko automatizációhoz - többek között tömeges NTP és Logging beállítása valamint automatizált konfiguráció mentés FTP szerverre
AllGPOs.pdf<br>ceopcresult.pdf<br>devpcresult.pdf<br>gplinkexports.pdf<br>groupmemberships.pdf<br>laci.itresult.pdf<br>pista.ceo_gpresult.pdf<br>sanyi.dev.1_gpresult.pdf<br>userlist.pdf | konfigurált +<br>exportált | - | - | Active Directory beállítások exportálása, bemutatva az érvényesülésüket és különbségeket

Vizsgaremek tesztelés.docx | Mindenki a saját munkáját tesztelte | A vizsgaremek tesztelése, bemutatva működését
------|-------|---------
Eszköz konfigurációk.docx | Mindenki a saját konfigurációját belemásolta | A konfigurációk kimásolva, hogy látható legyen pontosan mit állítottunk be
