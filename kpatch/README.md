# Demonstates using kpatch to keep a Kernel patched with no downtime

Slide Deck: https://docs.google.com/presentation/d/1QdloOPkqlpH1WsPnFoJqg0Z2-eU8K0wuQW0frbRRLIo/edit?usp=sharing

## Command List for this Demo

./tools/cve-2019-11135--2019-11-12-1735.sh
yum search 4.18.0-147.el8
yum install -y kpatch-patch-4_18_0-147.x86_64
kpatch list
./tools/cve-2019-11135--2019-11-12-1735.sh
yum update
./tools/cve-2019-11135--2019-11-12-1735.sh
uname -r
kpatch list
