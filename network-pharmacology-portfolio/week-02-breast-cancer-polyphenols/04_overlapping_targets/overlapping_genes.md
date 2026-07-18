# Daftar Target yang Beririsan

Berdasarkan diagram Venn (`venn_diagram.png`), terdapat **9 gen (2,2%)** yang beririsan antara 188 gen terkait Breast Cancer dan 207 target senyawa polifenol.

## Gen irisan yang membentuk jaringan PPI (6 dari 9)

Dari 9 gen irisan, 6 gen berikut membentuk jaringan interaksi (memiliki edge) di STRING/Cytoscape dan digunakan pada tahap analisis hub protein selanjutnya:

| No | Gene Symbol |
|----|-------------|
| 1 | CTNNB1 |
| 2 | PPARG |
| 3 | PTGS2 |
| 4 | PIK3CA |
| 5 | PARP1 |
| 6 | NFE2L2 |

> **Catatan:** 3 gen irisan lainnya merupakan node terisolasi (tanpa interaksi langsung dengan gen lain pada confidence STRING ≥ 0,4) sehingga tidak tampil pada jaringan PPI maupun tabel hub protein. Jika kamu punya daftar lengkap 9 gen dari hasil analisis Venn/STRING aslimu, lengkapi tabel ini dengan 3 gen yang belum tercantum.
