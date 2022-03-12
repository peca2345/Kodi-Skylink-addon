# Kodi Skylink IPTV addon

![obrazek](https://user-images.githubusercontent.com/58307338/158026556-d43929a6-232d-4852-afbb-b99b9cd78115.png)

**Konfigurace:**
- CoreELEC/LibreELEC 19.5
- Mecool KM9 Pro (S905X2 / 4GB RAM / 32GB ROM / Mali-G31 MP2)
- ELEC boot z USB3 flash disku

**Instalace:**

1. Vytvořte si účet Skylink a zaplaťte předplatné.  
2. Nainstalujte addon Skylink Live TV z CZ/SK repa [ZDE](https://kodi-czsk.github.io/repository/)    
3. V nastevení Skylinku vyberte Skylink CZ a zadejte login.  
4. Dále v nastavení playlist a EPG nastavte cestu do jakékoliv složky v zařízení.  
5. Po uložení nastavení se vygeneruje playlist a epg do zvoleného adresáře.  
6. Spusťte nějaký stream z addonu Skylink a tím se nainstaluje widevine.  
7. Nainstalujte addon PVR IPTV Simple client, otevřete nastavení, uložte ho a restartujte Kodi.    
8. Otevřete znovu Skylink addon/záložku PVR IPTV Simple client a klikněte na nastavení PVR IPTV Simple client.  
9. Tím se zkopírují cesty playlist a EPG ze Skylink do IPTV Simple client.  
9. Restartuje Kodi.  
	 
**Sekání streamu:**

Způsobuje to poslední verze winevide. Řešením je manuální downgrade nahrazením souboru v root adresáři Kodi.  
Problém detekován jen u CoreELEC. Na Windows a LibreELEC se neprojevuje.  
 
1. Povolte zobrezení skrytých souborů. (nastavení/media/obecné)  
2. Stáhněte starší verzi widevine. -> [ZDE](https://github.com/peca2345/Kodi-Skylink-addon/raw/main/libwidevinecdm.so)  
3. Zkopírujte do skrytého adresáře kodi. (správce souborů/přidat zdroj/procházet/kořenový souborový systém)  
4. V tomto zdroji najděte složku CDM a v ní nahraďte libwidevinecdm.so. (storage/.kodi/cdm)  
5. Restartujte Kodi  

**Skylink - nastavení:**   
- Účet / Poskytovatel - Skylink CZ    
- Playlist / umistění playlistu: /storage/twshows  
- EPG / umístění EPG: storage/twshows  
- Archiv / vše zapnout  
	
**InputStream Adaptive - nastavení:**  
- bez úprav - default    

**PVR IPTV Simple Client nastaveni:**   
- M3U playlist: /storage/tvshows/playlist.m3u  
- TV program: /storage/tvshows/epg.xml  
- Timeshift: all on  
- Catchup: all on  

**PVR a Živé vysílání:**
- Televizní program/výchozí akce při výběru/chytrý výběr  

**Tipy:**
- dlouhé podržení OK otevře přehledný seznam stanic na levé straně bez přerušení streamu
- při sledovaní LIVE streamu nejde přetáčet ale při streamu pořadu z archivu ano

**Zdroj:**
[xbmc-kodi.cz](https://www.xbmc-kodi.cz/prispevek-skylink-livetv-addon?fbclid=IwAR2LyNlfZMKUy_j3w_AsF4OOx0d-GKXujYZgzn4jzUnHn1rBzdClddwaD3I)  
