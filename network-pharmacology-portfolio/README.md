# Network Pharmacology & Molecular Docking Portfolio

Repository ini berisi kumpulan tugas dan project analisis *network pharmacology* dan *molecular docking* yang dikerjakan selama program pembelajaran, dan akan terus dikembangkan hingga Capstone Project.

## Daftar Isi

| Week | Topik | Link |
|------|-------|------|
| Week 2 | Identification of Therapeutic Targets and Molecular Mechanisms of Selected Plant-Derived Polyphenols Against Breast Cancer Using Network Pharmacology | [`week-02-breast-cancer-polyphenols/`](./week-02-breast-cancer-polyphenols/) |

## Tools & Database yang Digunakan

- **PubChem** — identifikasi senyawa
- **SwissTargetPrediction** — prediksi target protein
- **OMIM** — identifikasi target penyakit
- **STRING** — konstruksi Protein-Protein Interaction (PPI) Network
- **Cytoscape** (cytoHubba) — visualisasi network dan identifikasi hub protein
- **ShinyGO / Metascape** — enrichment analysis (GO & KEGG pathway)

## Struktur Folder per Week

Setiap folder week mengikuti struktur berikut:

```
week-XX-topik/
├── README.md                  # Ringkasan & ketentuan tugas
├── 01_compound_identification/
├── 02_target_prediction/
├── 03_disease_targets/
├── 04_overlapping_targets/
├── 05_ppi_network/
├── 06_cytoscape_visualization/
├── 07_hub_proteins/
├── 08_enrichment_analysis/
├── 09_workflow_diagram/
└── [NomorKelompok]_[NamaPeserta]_WeekXX.md   # Laporan interpretasi hasil
```
