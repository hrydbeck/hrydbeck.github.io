# How Mimosa can access clustering distances

The plan for Mimosa is to build a cluster tree that grows with submitted samples?
Newly submitted samples are positioned in the clustertree. Not realistic to cluster too many samples. A similarity cutoff is specifed. If samples are identical/very similar and outbreak warning is indicated.

The clustering will indicative and needs validation with more accurate clustering possibly with Bonsai.

Agnostic approach?

## Mimosa access Bonsai API

Access through http://ip-adress:8001/docs. 

Bonsai använder Grapetree för att visualisera clustring

### Issues

Bonsai will not store any clustering information.
A set of samples can be provide to the custer API for clustering.
A cluster tree in Newick formmat wil be returned.


## Add clustering functionality to Jasen

Could possibly use jasen output directly

Can still use Bonsai for  quality check. can add commets that can later be accessed by API

### [Enterobase hierarcical clustering](https://enterobase.warwick.ac.uk/)


Hierarcical clustering, nomenclatur??

Entrobase hieracical clustering, funkar isåfall bara för cgmlst data

Gjorde Public Health England för 5 år sedan med snp data. Skapa mumericclustre(?). Är adressen identisk så är det inga skillnader.
Sträng med integers som man kan filtrera på.

https://enterobase.warwick.ac.uk/


Add clustergroup in Jasen ?


Hierarkisk clustering är på väg in i Jasen. Inom ett halvår kan Hierrkisk klustring vara på plats

Agens mikrobiology = patogener



## Halfdan kolla på 
- Kolla Jasen repot och se hur det är upplagt
- Nextflow DSL2 används
- Kolla hur Enterobase gör klustring
