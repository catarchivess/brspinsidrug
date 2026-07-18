# Week 2 — Network Pharmacology: Plant-Derived Polyphenols vs Breast Cancer

**Judul:** Identification of Therapeutic Targets and Molecular Mechanisms of Selected Plant-Derived Polyphenols Against Breast Cancer Using Network Pharmacology

**Senyawa:** Resveratrol, Kaempferol, Luteolin, Genistein, Quercetin, Apigenin
**Target penyakit:** Breast Cancer

## Isi Folder

| Folder / File | Isi |
|---|---|
| `01_compound_identification/` | Daftar senyawa dari PubChem |
| `02_target_prediction/` | Tabel target protein hasil SwissTargetPrediction |
| `03_disease_targets/` | Tabel target penyakit hasil OMIM |
| `04_overlapping_targets/` | Diagram Venn & daftar gen yang beririsan |
| `05_ppi_network/` | Screenshot & data PPI Network dari STRING |
| `06_cytoscape_visualization/` | Screenshot visualisasi network dari Cytoscape (termasuk merged network) |
| `07_hub_proteins/` | Tabel hub protein (degree, betweenness, closeness centrality) |
| `08_enrichment_analysis/` | Visualisasi enrichment analysis (GO & KEGG pathway) |
| `09_workflow_diagram/` | Diagram alur (flowchart) workflow analisis |
| `[NomorKelompok]_[NamaPeserta]_Week2.md` | **Laporan interpretasi hasil (500-800 kata)** |

## Ringkasan Alur Analisis

1. Identifikasi senyawa (PubChem) → 6 senyawa polifenol
2. Prediksi target protein (SwissTargetPrediction)
3. Identifikasi target penyakit (OMIM) → gen terkait Breast Cancer
4. Irisan target senyawa & penyakit → 9 gen
5. Konstruksi PPI Network (STRING)
6. Visualisasi network (Cytoscape)
7. Identifikasi hub protein (Degree Centrality, cytoHubba) → CTNNB1, PPARG, PTGS2 sebagai top 3
8. Enrichment analysis (KEGG pathway) → EGFR-TKI resistance, PI3K-Akt signaling, Ras signaling, dll.
9. Interpretasi hasil

Detail lengkap ada di file laporan interpretasi hasil.
