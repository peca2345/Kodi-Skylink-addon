# Kodi Skylink IPTV addon

**Instalace:**

1. registrovat skylink a zaplatit  
2. nainstalovat addon skylink  
3. otevřít nastavení a nastavit pevné cesty pro playlist a epg v lokální složce zařizení  
4. po uložení nastavení se vygeneruje playlist a epg 
5. nainstalovat PVR IPTV simple client addon  
6. otevřít znovu skylink addon a otevřít záložku PVR IPTV Simple client a kliknout na nastavení  
	 tim se nastavi IPTVsimpleclient na hodnoty ze skylink addonu  
7. v hlavním nastavení / media / obecné / povolit zobrazení skrytých adresářů  
8. stáhnout starší verzi widevine (s novou se všechno seká a nestíhá buffer)  
	      https://k.slyguy.xyz/.decryptmodules/widevine/4.10.2252.0-linux-armv7.so  
9. přejmenovat 4.10.2252.0-linux-armv7.so na libwidevinecdm.so  
10. zkopirovat do root skrytého adresáře kodi  
	      správce souborů / přidat zdroj / procházet/ kořenový souborový systém  
11. v tomto zdroji najit složku cdm a v ní nahradit libwidevinecdm.so tim co jsi stáhnul  
	      storage / .kodi / cdm /   
12. restartovat kodi  

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
