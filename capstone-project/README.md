# Capstone Project — In Silico Drug Discovery

**Topik:** Identifikasi Target Terapeutik dan Mekanisme Molekuler Polifenol Tumbuhan terhadap Breast Cancer Melalui Pendekatan Network Pharmacology dan Molecular Docking

**Peserta:** Calista Aqilah Tsabitah (individu)

## Ringkasan Project

Enam senyawa polifenol tumbuhan (Quercetin, Luteolin, Kaempferol, Apigenin, Genistein, Resveratrol) dianalisis mekanisme kerjanya terhadap breast cancer melalui integrasi network pharmacology (identifikasi hub gene) dan molecular docking (validasi struktural).

**Temuan utama:**
- 9 gen irisan antara target senyawa (207 gen) dan target breast cancer OMIM (197 gen); 6 gen membentuk jaringan PPI
- **CTNNB1 (β-catenin)** — hub gene #1 (Degree 4) → didocking dengan **Quercetin** → binding affinity −6.7 kcal/mol pada groove TCF4-binding
- **PPARG** — hub gene #2 (Degree 3) → didocking dengan **Genistein** → binding affinity −8.7 kcal/mol pada ligand-binding pocket
- Enrichment KEGG: EGFR-TKI resistance, PI3K-Akt signaling, Ras signaling, Breast cancer pathway

## Struktur Folder

```
capstone-project/
├── CalistaAqilahTsabitah_CapstoneReport.pdf   ← laporan utama (baca ini dulu)
├── CalistaAqilahTsabitah_CapstoneReport.docx
├── network-pharmacology/                       ← Hasil analisis Week 2
│   ├── senyawadantarget.csv                     (raw SwissTargetPrediction)
│   ├── breastcancergenome_fromOMIM.csv          (daftar target penyakit)
│   ├── intersecting_genes_table.png             (9 gen irisan → 6 gen ber-edge)
│   ├── hub_gene_ranking_degree.png              (ranking cytoHubba)
│   ├── ppi_network_cytoscape.png                (visualisasi network)
│   ├── merged_network_enrichment.png            (network gabungan + pathway)
│   └── week2_interpretation.md                  (laporan interpretasi Week 2)
├── molecular-docking/                           ← Hasil docking Week 3 (2 target)
│   ├── ctnnb1_1jdh/
│   │   ├── CurPockets_info.txt                  (hasil blind docking CB-Dock2)
│   │   ├── quercetin_pose_surface.png
│   │   └── quercetin_pose_cartoon.png
│   └── pparg_1prg/
│       ├── CurPockets_info_1PRG.txt
│       └── genistein_pose_cavity1.png
└── video/
    └── link_video_presentasi.md                 ← link video (isi setelah upload)
```

## Tools yang digunakan

- **Network Pharmacology:** SwissTargetPrediction, OMIM, STRING, Cytoscape (cytoHubba), ShinyGO/Metascape
- **Molecular Docking:** RCSB PDB, PubChem, CB-Dock2 (AutoDock Vina) — digunakan sebagai alternatif SwissDock yang mengalami kendala akses server saat pengerjaan
