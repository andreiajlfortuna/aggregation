# Aggregation

### FTIR simulation

e.g. with two structures from the most populated cluster

- Convert pdb structures into xyz to extract the coordinates

obabel structure1.pdb -O structure1.xyz

Optimization must have the keywords: 
#p B3LYP/6-31G(d,p) Int=UltraFine Opt=tight SCRF=(PCM,Solvent=EthylEthanoate)

g16 opt.com

Frequency calculation:
#p B3LYP/6-31G(d,p) Freq Int=UltraFine SCRF=(PCM,Solvent=EthylEthanoate) Geom=AllCheck Guess=Read
