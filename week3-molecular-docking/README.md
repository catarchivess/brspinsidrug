# Week 3 — Molecular Docking

Replikasi workflow molecular docking: memvalidasi interaksi antara hub gene hasil Week 2 (CTNNB1) dengan salah satu senyawa polifenol kandidat (Quercetin).

## Ringkasan

| | |
|---|---|
| Protein target | CTNNB1 (β-catenin), PDB 1JDH, chain A, resolusi 2.0 Å |
| Ligan | Quercetin (SMILES dari PubChem CID 5280343) |
| Tools | CB-Dock2 (blind docking, AutoDock Vina) — alternatif SwissDock yang mengalami kendala server |
| Cavity terpilih | Cavity 4 (skor −6.7 kcal/mol; residu kontak beririsan dengan situs TCF4-binding groove) |

## Isi Folder

- `5_CalistaAqilahTsabitah_Week3.pdf` / `.docx` — laporan lengkap (info protein-ligan, konfigurasi docking, hasil binding affinity, visualisasi, interpretasi)
- `data/CurPockets_info_CTNNB1.txt` — output mentah deteksi cavity dari CB-Dock2
- `visuals/` — screenshot visualisasi 3D pose docking (representasi permukaan & cartoon)
