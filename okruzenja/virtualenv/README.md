# Virtualenv  

<a href="https://virtualenv.pypa.io/en/stable/">Virtualenv</a> je alat za kreiranje izolovanih (virtuelnih) *Python* okruženja. Vrši kreiranje okruženja koje ima sopstvene instalacione direktorijume, i koje ne deli pakete sa ostalim okruženjima (uključujući i globalno instalirane pakete).  

## Podešavanje i upotreba

### Linux i MacOS

1. Instalirati <a href="https://www.python.org/downloads/">Python 3.6.x i pip3</a>.  
**Napomena:** biblioteke koje će se koristiti bi trebale biti kompatibilne sa *Python 3.4+*. 

2. Instalirati *virtualenv*:  
`$ pip install virtualenv`  

3. U sklopu proizvoljnog foldera kreirati virtuelno okruženje:  
`$ cd my_folder/`  
`$ virtualenv env` 

4. Aktivirati kreirano virtuelno okruženje i instalirati neophodne pakete:  
`$ source env/bin/activate`  
`$ pip install -r requirements.txt`

Nakon izvršenja poslednje komande, podešavanje virtuelnog okruženja je kompletirano, i ono ostaje aktivirano za (eventualni) dalji rad.

Pre početka rada sa virtuelnim okruženjem, neophodno je pozicionirait se u folder u kom je kreiran, i aktivirati ga:  
`$ cd my_folder/`  
`$ source env/bin/activate`  

Nakon završetka rada, virtuelno okruženje se deaktivira pomoću sledeće komande:  
`$ deactivate`  

Instalacija novog paketa se vrši pomoću:  
`$ pip install ime_paketa`  

Ažuriranje liste instaliranih paketa u okržuenju (**requirements.txt**) se vrši pomoću sledeće komande:  
`$ pip freeze > requirements.txt`  


### Windows  

Na *Windows* operativnom sistemu podešavanja i upotreba su analogna podešavanju i upotrebi na *Linux* i *MacOS* operativnim sistemima. Jedina razlika jeste prilikom aktiviranja i deaktiviranja okruženja.

Prilikom kreiranja okruženja na *Windows* operativnom sistemu se kreiraju aktivacione skripte za *Command Prompt* i *Powershell*, zbog toga se aktivacija okruženja na *Windows*-u vrši pomoću sledeće komande:  
`> \path\to\env\Scripts\activate`  
Deaktivacija se vrši pomoću sledeće komande:  
`> deactivate`  

Više informacija o radu sa *virtualenv*-om na *Windows*-u možete pronaći <a href="https://virtualenv.pypa.io/en/stable/userguide/#windows-notes">ovde</a>.
