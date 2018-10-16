# Anaconda

<a href="https://www.anaconda.com/distribution/">Anaconda Distribution</a> predstavlja *open source* distribuciju za najbrži i najlakši rad sa *AI*-om i *Data Science*-om u programskim jezicima *R* i *Python* na *Linux*, *Windows* i *MacOS*  operativnim sistemima. Predstavlja industrijski standard za razvoj, testiranje i trening na jednom računaru.  

## Instalacija

Za potrebe ovog kursa potrebno je instalirati **Anaconda 5.2.0 sa Python 3.6**.  
Potrebno je sa sledećeg <a href="https://repo.anaconda.com/archive/">linka</a> preuzeti fajl **Anaconda3-5.2.0-** za željeni operativni sistem (npr.: za *Linux 64-bit* fajl je: **Anaconda3-5.2.0-Linux-x86_64.sh**) i pratiti uputstva za instalaciju koja se mogu pronaći <a href="http://docs.anaconda.com/anaconda/install/">ovde</a>.  

Instalacija se može verifikovati pomoću:  
`$ conda --version`  
Ukoliko je instalacija bila uspešna, dobiće se ispis oblika: **conda 4.x.y**.

Alternativni načini za instalaciju *Anaconda*-e sa *Python 3.6* se mogu pronaći <a href="http://docs.anaconda.com/anaconda/faq/#id4">ovde</a>.

Spisak dostupnih paketa se nalazi <a href="https://docs.anaconda.com/anaconda/packages/pkg-docs/">ovde</a>.


## Conda  

Distribucija uključuje <a href="https://conda.io/docs/index.html">Conda Data Science Package & Environment Manager</a> koji  
omogućava laku instalaciju i održavanje preko 1400 *Python* i *R* paketa. *Conda* omogućava olakšan rad sa okruženjima na računaru.

### Kreiranje okruženja  

Okruženje potrebno za ovaj kurs se kreira na sledeći način:  
1. Instalacija dodatnih paketa:  
`$ conda install opencv tensorflow keras`  

2. (opciono) Provera instaliranih paketa:  
`$ conda list`  

3. Kreiranje okruženja pod nazivom *soft*:  
`$ conda create -n soft`  

### Rad sa okruženjem

1. Pre početka rada sa paketima u sklopu okruženja, potrebno je aktivirati okruženje:  
* *Linux* i *MacOS*:  
`$ source activate soft`  
* *Windows*:  
u *Anaconda Prompt*-u kucati:  
`$ activate soft`  

2. Nakon završetka rada, okruženje se deaktivira:  
* *Linux* i *MacOS*:  
`$ source deactivate`  
* *Windows*:  
u *Anaconda Prompt*-u kucati:  
`$ deactivate`  

Ostatak komandi za rad sa *Conda*-om je dostupan <a href="https://conda.io/docs/user-guide/index.html">ovde</a>.

## Anaconda Navigator  

<a href="http://docs.anaconda.com/anaconda/navigator/">Anaconda Navigator</a> predstavlja *GUI* uključen u *Anaconda* distribuciju koji omogućava poretanje aplikacija, rad sa paketima i okruženjima bez korišćenja komandne linije. Predstavlja svojevrsnu alternativu za *Conda*-u. Pokreće se pomoću komande:  
`$ anaconda-navigator`
