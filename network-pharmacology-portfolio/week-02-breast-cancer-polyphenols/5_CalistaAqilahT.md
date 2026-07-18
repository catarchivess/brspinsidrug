# Laporan Interpretasi Hasil — Week 2

**Topik:** Identification of Therapeutic Targets and Molecular Mechanisms of Selected Plant-Derived Polyphenols Against Breast Cancer Using Network Pharmacology

**Senyawa:** Resveratrol, Kaempferol, Luteolin, Genistein, Quercetin, Apigenin
**Penyakit:** Breast Cancer

---

## Bagaimana mekanisme molekuler senyawa polifenol dalam memengaruhi Breast Cancer, dilihat dari hub protein sentral dan pathway biologis hasil enrichment analysis?

Enam senyawa polifenol tumbuhan (Resveratrol, Kaempferol, Luteolin, Genistein, Quercetin, dan Apigenin) diprediksi target proteinnya menggunakan SwissTargetPrediction, kemudian diirisankan dengan daftar gen terkait *breast cancer* dari OMIM. Hasil diagram Venn menunjukkan 188 gen spesifik terkait *breast cancer* (46,5%), 207 gen merupakan target spesifik senyawa (51,2%), dan 9 gen (2,2%) merupakan irisan keduanya. Kesembilan gen irisan inilah yang menjadi kandidat target kerja senyawa polifenol terhadap *breast cancer*, dan selanjutnya dikonstruksi menjadi jaringan *Protein-Protein Interaction* (PPI) melalui STRING.

Dari 9 gen irisan, hanya 6 gen yang membentuk jaringan interaksi dengan tautan (edge) satu sama lain, yaitu **CTNNB1, PPARG, PTGS2, PIK3CA, PARP1,** dan **NFE2L2**; sisanya merupakan node terisolasi tanpa interaksi langsung. Analisis *degree centrality* menggunakan cytoHubba pada Cytoscape mengidentifikasi **CTNNB1 (β-catenin)** sebagai hub protein paling sentral, dengan nilai degree tertinggi (4,0), diikuti nilai *betweenness centrality* (0,70) dan *closeness centrality* (0,83) yang juga tertinggi dibandingkan protein lain dalam jaringan. Hub protein berikutnya adalah **PPARG** (degree 3,0; betweenness 0,40) dan **PTGS2** (degree 2,0), sementara PIK3CA, PARP1, dan NFE2L2 masing-masing memiliki degree 1,0. Tingginya nilai sentralitas CTNNB1 mengindikasikan bahwa protein ini berperan sebagai penghubung utama dalam jaringan interaksi antarprotein, sehingga kemungkinan besar menjadi target kunci yang memediasi efek multi-target senyawa polifenol terhadap sel kanker payudara.

Secara biologis, CTNNB1 adalah komponen inti jalur **Wnt/β-catenin**, jalur sinyal yang mengatur proliferasi, diferensiasi, dan kelangsungan hidup sel, dan sering mengalami disregulasi pada kanker payudara sehingga mendorong pertumbuhan tumor yang tidak terkendali. PPARG (*peroxisome proliferator-activated receptor gamma*) berperan dalam regulasi diferensiasi sel dan metabolisme lipid, di mana aktivasinya oleh senyawa polifenol dapat menghambat proliferasi sel kanker dan mendorong diferensiasi ke arah fenotip yang kurang ganas. Sementara itu, PTGS2 (COX-2) merupakan enzim kunci dalam jalur inflamasi yang berkontribusi terhadap progresi tumor, angiogenesis, dan resistensi terhadap apoptosis; penghambatan PTGS2 oleh polifenol seperti quercetin dan apigenin telah banyak dilaporkan menekan inflamasi terkait tumor.

Hasil *enrichment analysis* KEGG pathway terhadap 6 gen hub tersebut menunjukkan keterlibatan sejumlah jalur onkogenik dengan nilai *fold enrichment* tertinggi pada **EGFR tyrosine kinase inhibitor resistance** (≈190), diikuti oleh jalur-jalur signifikan lain seperti **PI3K-Akt signaling pathway, Ras signaling pathway, Focal adhesion, Rap1 signaling pathway**, serta jalur yang secara spesifik berkaitan dengan *Breast cancer*. Keterlibatan jalur PI3K-Akt dan Ras/MAPK sejalan dengan peran sentral PIK3CA dan CTNNB1 sebagai regulator proliferasi dan kelangsungan hidup sel kanker, sedangkan keterkaitan dengan jalur resistensi EGFR-TKI mengindikasikan bahwa target-target ini juga relevan dalam konteks sensitivitas sel kanker terhadap terapi target molekuler yang sudah ada.

Secara keseluruhan, mekanisme molekuler senyawa polifenol terhadap *breast cancer* dapat dijelaskan melalui kerja multi-target pada tiga simpul utama: **CTNNB1** (jalur Wnt/β-catenin, proliferasi dan kelangsungan hidup sel), **PPARG** (diferensiasi sel dan metabolisme), serta **PTGS2** (inflamasi dan progresi tumor). Ketiganya saling terhubung dalam jaringan PPI dan secara kolektif memodulasi jalur PI3K-Akt dan Ras signaling yang teridentifikasi melalui enrichment analysis. Pola ini memperkuat gagasan bahwa senyawa polifenol tumbuhan bekerja bukan melalui satu target tunggal, melainkan melalui efek sinergis pada beberapa jalur onkogenik yang saling terkait, menjadikan CTNNB1, PPARG, dan PTGS2 sebagai kandidat target terapeutik utama yang berpotensi divalidasi lebih lanjut melalui studi *in vitro* maupun *in vivo*, termasuk melalui pendekatan *molecular docking* pada tahap analisis berikutnya.

---

**Jumlah kata:** ±510 kata

## Referensi

1. Rabbani, S. A., Sharma, S., El-Tanani, M., Khurana, S., Saini, M., Yadav, M., Kumar, R., & El-Tanani, Y. (2026). Plant-derived polyphenols in cancer therapy: Bridging molecular mechanisms and bioavailability toward clinical translation. *Pharmaceutics*, 18(6), 737. https://doi.org/10.3390/pharmaceutics18060737
2. Rakoczy, K., Kaczor, J., Sołtyk, A., Szymańska, N., Stecko, J., Sleziak, J., et al. (2023). Application of luteolin in neoplasms and nonneoplastic diseases. *International Journal of Molecular Sciences*, 24(21), 15995. https://doi.org/10.3390/ijms242115995
