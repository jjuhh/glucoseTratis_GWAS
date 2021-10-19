# glucoseTratis_GWAS

## LD check using list of SNPs
```
for i in {1..22}
do echo $i
plink --bfile Chr${i}.genotype --out chr${i}.LD --threads 30 --tag-kb 1000 --tag-r2 0.6 --show-tags snp.list --list-all
done
```
