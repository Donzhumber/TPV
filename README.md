# Submission Package: Terrorism and Political Violence (TPV)

**Manuscript Title:** *Identifying Rational Types in Unknown Environments under an Indirect Dynamic Mechanism*  
**Author:** Prof. Humberto Bernal, Ph.D.  
**Target Journal:** *Terrorism and Political Violence* (TPV)  
**Publisher:** Routledge / Taylor & Francis  
**Editor-in-Chief:** Prof. James J.F. Forest (University of Massachusetts Lowell)  
**Submission Portal:** [ScholarOne Manuscripts (https://mc.manuscriptcentral.com/ftpv)](https://mc.manuscriptcentral.com/ftpv)  
**Submission Fee:** **$0 (Zero submission fee — standard Routledge / Taylor & Francis policy)**  
**Peer Review Mode:** Double-Blind Peer Review  
**Abstract Length:** 88 words  
**Keywords:** indirect mechanism design; dynamic screening; endogenous implementation noise; Bayesian learning; type identification; counter-terrorism policy; political violence; insurgency dynamics  
**JEL Codes:** C73 (Stochastic and Dynamic Games); D82 (Asymmetric and Private Information / Mechanism Design); K42 (Illegal Behavior and the Enforcement of Law)  
**Replication Repository:** [https://github.com/Donzhumber/TPV.git](https://github.com/Donzhumber/TPV.git)  
**Interactive Simulator:** [https://7kkgn4sfscykkfvv5794qw.streamlit.app/](https://7kkgn4sfscykkfvv5794qw.streamlit.app/)

---

## 1. Ready-to-Upload Submission Package (`UPLOAD_FILES/`)

All files required for submission via ScholarOne Manuscripts are compiled, verified, and sequentially organized in the `UPLOAD_FILES/` directory:

| Item / File Name | ScholarOne File Designation | Description & Document Role | Size |
| :--- | :--- | :--- | :--- |
| `01_MANUSCRIPT_TPV_Anonymous.pdf` | **Main Document** | Blinded manuscript for double-blind peer review (author details omitted) | ~3.4 MB |
| `01b_MANUSCRIPT_TPV_Named.pdf` | **Supplemental File NOT for Review** | Full archival manuscript with author credentials, affiliations, and statements | ~3.4 MB |
| `02_Title_Page_TPV.pdf` | **Title Page** | Standalone title page (author details, abstract, keywords, declarations) | ~62 KB |
| `03_Cover_Letter_TPV.pdf` | **Cover Letter** | Addressed to Prof. James J.F. Forest, Editor-in-Chief (*TPV*) | ~113 KB |
| `04_Highlights_TPV.pdf` | **Highlights** | 5 research highlights emphasizing political violence and policy trade-offs | ~63 KB |
| `05_Declaration_of_Interest_TPV.pdf` | **Declaration of Interest** | Formal statement declaring no competing financial or personal interests | ~73 KB |
| `06_Authorship_Statement_TPV.pdf` | **Authorship Statement** | Authorship contribution statement for Humberto Bernal (sole author) | ~73 KB |
| `07_Supplementary_Appendix_A.zip` | **Supplemental File** | Econometric calibration: Stata 19 `.do` scripts, analytical microdata, outputs | ~6.6 MB |
| `08_Supplementary_Appendix_B.zip` | **Supplemental File** | Formal mathematical proofs & Lean 4 interactive theorem prover project | ~539 KB |
| `09_Supplementary_Appendix_C.zip` | **Supplemental File** | Streamlit simulation tool, PyTorch neural network weights, Python modules | ~2.7 MB |
| `tpv_submission_metadata.txt` | **Metadata Guide** | Plain text guide for copy-pasting metadata into ScholarOne web forms | ~10 KB |

---

## 2. Directory Architecture

```
TPV/
├── README.md                                  # Master guide and submission documentation
├── .gitignore                                 # Git configuration ignoring build junk while tracking assets
├── UPLOAD_FILES/                              # Sequentially numbered submission deliverables
│   ├── 01_MANUSCRIPT_TPV_Anonymous.pdf        # Blinded Main Document
│   ├── 01b_MANUSCRIPT_TPV_Named.pdf           # Named Reference Manuscript
│   ├── 02_Title_Page_TPV.pdf                  # Standalone Title Page
│   ├── 03_Cover_Letter_TPV.pdf                # Cover Letter to Prof. James J.F. Forest
│   ├── 04_Highlights_TPV.pdf                  # 5 Research Highlights
│   ├── 05_Declaration_of_Interest_TPV.pdf     # Conflict of Interest Statement
│   ├── 06_Authorship_Statement_TPV.pdf        # Authorship Statement
│   ├── 07_Supplementary_Appendix_A.zip        # Stata Replication Package (Appendix A)
│   ├── 08_Supplementary_Appendix_B.zip        # Lean 4 Formal Proofs Package (Appendix B)
│   ├── 09_Supplementary_Appendix_C.zip        # Streamlit App & PyTorch Models (Appendix C)
│   └── tpv_submission_metadata.txt            # Formatted ScholarOne metadata
├── main/                                      # Main manuscript LaTeX source and assets
│   ├── Bernal_H_TPV_Anonymous.tex             # Blinded LaTeX source
│   ├── Bernal_H_TPV_Name.tex                  # Named LaTeX source
│   ├── title_page.tex                         # Title page source
│   ├── references.bib                         # BibTeX bibliography database
│   ├── elsarticle.cls / sn-jnl.cls            # Document classes
│   └── Figures/                               # High-resolution figures and maps
├── additional_documents/                      # Submission documentation sources
│   ├── cover_letter.tex / _ES.tex             # English & Spanish cover letters
│   ├── highlights.tex / _ES.tex               # English & Spanish research highlights
│   ├── declaration_of_interest.tex / _ES.tex  # Conflict of interest statements
│   └── authorship_statement.tex               # Authorship contribution statement
├── appendix_A_micro/                          # Supplementary Appendix A (Microeconometric Calibration)
│   ├── Appendix_A_Micro.tex                   # LaTeX source (20 pages)
│   ├── Appendix_A_Micro.pdf                   # Compiled PDF (20 pages)
│   ├── tables_mnl_full.tex / tables_cox_full.tex
│   └── scripts/                               # Stata .do files, data/Data_merge.dta, outputs
├── appendix_B_proofs/                         # Supplementary Appendix B (Formal Proofs & Lean 4)
│   ├── Appendix_B_Proofs.tex                  # LaTeX source (30 pages)
│   ├── Appendix_B_Proofs.pdf                  # Compiled PDF (30 pages)
│   ├── README.txt                             # Lean 4 replication guide
│   ├── replicate.sh                           # Build script for Lean project
│   └── lean/                                  # Lean 4 project (AppendixBProofs.lean, lakefile, toolchain)
└── Appendix_C_Streamlit/                      # Supplementary Appendix C (Deep Learning Simulation)
    ├── Appendix_C_Streamlit.tex               # LaTeX source (15 pages)
    ├── Appendix_C_Streamlit.pdf               # Compiled PDF (15 pages)
    ├── app_DL.py                              # Streamlit application entry point
    ├── dl_engine.py / dl_mechanism.py         # Computational logic modules
    └── captor_value_net_T10*.pt               # Trained PyTorch MLP value networks
```

---

## 3. Taylor & Francis / TPV Submission Guidelines Compliance

1. **Zero Submission Fee ($0):**  
   *Terrorism and Political Violence*, published by Routledge / Taylor & Francis, operates on a standard subscription / hybrid open-access model. Submitting a manuscript to TPV entails **$0 in submission or peer review fees**.

2. **Double-Blind Peer Review:**  
   - **Blinded Manuscript (`01_MANUSCRIPT_TPV_Anonymous.pdf`):** Designated as "Main Document" in ScholarOne. Contains no author names, affiliations, email addresses, or self-identifying funding acknowledgments. Self-citations and repository references are fully anonymized.
   - **Title Page (`02_Title_Page_TPV.pdf`):** Designated as "Title Page" in ScholarOne. Contains author names, institutional affiliations, ORCID identifier, corresponding author contact details, abstract, keywords, and declarations.
   - **Archival Named Manuscript (`01b_MANUSCRIPT_TPV_Named.pdf`):** Designated as "Supplemental File NOT for Review" for editorial reference.

3. **Scope and Editorial Focus:**  
   The paper directly addresses TPV's core thematic areas:
   - **Strategic dynamics of insurgent and terrorist organizations:** Analyzes Colombian guerrilla cells (FARC, ELN) and paramilitary groups (AUC).
   - **Information asymmetry & clandestine screening:** Models how states identify latent insurgent types under observational pooling and operational noise.
   - **Counter-terrorism policy design:** Evaluates the empirical and theoretical trade-offs between financial asset interdiction ($\alpha$) and tactical kinetic pressure ($\gamma$).

4. **ScholarOne Step-by-Step Upload Instructions:**  
   When submitting at [https://mc.manuscriptcentral.com/ftpv](https://mc.manuscriptcentral.com/ftpv):
   - **Step 1: Type, Title, & Abstract:** Paste title and abstract from `tpv_submission_metadata.txt`.
   - **Step 2: File Upload:** Upload all 10 numbered files matching the designations listed in Section 1.
   - **Step 3: Attributes:** Add keywords and select relevant subject classifications.
   - **Step 4: Authors & Institutions:** Humberto Bernal (Sole author & Corresponding author).
   - **Step 5: Reviewers:** Suggest appropriate theoretical and conflict studies reviewers.
   - **Step 6: Details & Comments:** Paste Cover Letter text, confirm conflict of interest, and add comments to editor.
   - **Step 7: Review & Submit:** Verify generated PDF proof and submit.

---

## 4. Replication and Verification

- **Lean 4 Verification (Appendix B):**
  ```bash
  cd appendix_B_proofs
  ./replicate.sh
  ```
- **Stata Replication (Appendix A):**
  ```bash
  cd appendix_A_micro/scripts
  stata -b do run_all.do
  ```
- **Streamlit Interactive Application (Appendix C):**
  ```bash
  cd Appendix_C_Streamlit
  streamlit run app_DL.py
  ```
  Or visit the web deployment: [https://7kkgn4sfscykkfvv5794qw.streamlit.app/](https://7kkgn4sfscykkfvv5794qw.streamlit.app/).
