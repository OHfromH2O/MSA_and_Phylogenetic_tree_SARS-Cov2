# MSA_and_Phylogenetic_tree_SARS-Cov2

### Practicals on computational biology
: created multiple sequence alignment (MSA) of spike proteins of different SARS-Cov-2 variants with clustalw2, as well as basic phylogenetic trees by fasttree.

# 🦠 SARS-CoV-2 다중 서열 정렬(MSA) 및 계통수 분석
**Computational Biology Lab Assignment**

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/python-3.x-blue.svg)
![Biopython](https://img.shields.io/badge/library-Biopython-orange.svg)

## 📌 프로젝트 개요 (Overview)
본 레포지토리는 컴퓨팅 생물학(Computational Biology) 실습 과제의 일환으로 진행된 **SARS-CoV-2(코로나19 바이러스) 유전체 서열의 다중 서열 정렬(MSA, Multiple Sequence Alignment) 및 계통수(Phylogenetic Tree) 구축 프로젝트**입니다. 

다양한 지역 및 시기에서 수집된 SARS-CoV-2의 염기서열(또는 단백질 서열)을 비교 분석하여, 바이러스의 진화적 연관성과 주요 변이 양상을 구조적으로 시각화하는 것을 목표로 합니다.

## 🎯 분석 목표 (Objectives)
1. **서열 전처리:** NCBI/GISAID 데이터베이스로부터 SARS-CoV-2 서열(FASTA 형식) 수집 및 정제
2. **다중 서열 정렬 (MSA):** 상동성(Homology) 비교를 통해 서열 간의 보존 영역(Conserved region)과 변이(Mutation) 위치 식별
3. **계통수 구축 (Phylogenetic Analysis):** 정렬된 서열을 바탕으로 진화적 거리를 계산하여 계통수를 시각화하고, 클레이드(Clade) 간의 연관성 분석

## 🛠️ 사용된 도구 및 파이프라인 (Methods & Tools)
> 💡 *실제 실습에서 사용한 도구만 남기고 삭제/수정하세요.*
* **데이터 소스:** [NCBI Virus / GISAID]
* **MSA 도구:** Clustal Omega / MAFFT / MUSCLE
* **계통수 구축 알고리즘:** Neighbor-Joining (NJ) / Maximum Likelihood (ML) 알고리즘 (사용 도구: MEGA / IQ-TREE / FastTree 등)
* **시각화 툴:** FigTree / iTOL (Interactive Tree Of Life) / Python (Matplotlib, Biopython)
* **사용 언어:** Python (또는 R, Bash)

## 📁 레포지토리 구조 (Repository Structure)
```text
MSA_and_Phylogenetic_tree_SARS-Cov2/
│
├── data/                  # 원본 및 전처리된 FASTA 서열 데이터
│   ├── raw_sequences/     # NCBI 등에서 다운로드한 원본 파일
│   └── aligned_data/      # MSA(다중 서열 정렬)가 완료된 파일 (.aln, .fasta)
│
├── scripts/               # 분석에 사용된 Python/R 스크립트 코드
│   ├── 01_data_prep.py    # 데이터 전처리 코드
│   ├── 02_run_MSA.py      # 서열 정렬 실행 코드
│   └── 03_build_tree.py   # 계통수 구축 및 시각화 코드
│
├── results/               # 최종 산출물 및 시각화 이미지
│   ├── phylogenetic_tree.png  # 완성된 계통수 이미지 파일
│   └── tree_file.nwk          # 시각화 툴에서 열 수 있는 Newick 트리 파일
│
└── README.md              # 프로젝트 설명 문서
📊 주요 분석 결과 (Key Results)
(분석 후 도출된 핵심 결과나 인사이트를 요약해서 적어주세요. 계통수 이미지를 첨부하면 아주 좋습니다!)

계통수 시각화: <img src="results/phylogenetic_tree.png" width="600" alt="SARS-CoV-2 Phylogenetic Tree">

분석 요약: * 분석 결과, 특정 변이(예: Omicron, Delta)가 기존 염기서열 그룹과 명확하게 분기(Clade)됨을 확인했습니다.

특히 스파이크(Spike) 단백질 서열 영역 부근에서 집중적인 변이가 관찰되었습니다.

🚀 실행 방법 (Usage)
이 프로젝트를 로컬 환경에서 재현하려면 아래 단계를 따르세요.

1. 레포지토리 클론

Bash
git clone [https://github.com/OHfromH2O/MSA_and_Phylogenetic_tree_SARS-Cov2.git](https://github.com/OHfromH2O/MSA_and_Phylogenetic_tree_SARS-Cov2.git)
cd MSA_and_Phylogenetic_tree_SARS-Cov2
2. 필요 패키지 설치

Bash
pip install biopython matplotlib pandas
3. 스크립트 실행

Bash
# 데이터 전처리 및 MSA 실행
python scripts/02_run_MSA.py

# 계통수 구축
python scripts/03_build_tree.py
👨‍💻 Author
GitHub: @OHfromH2O

Course: [과목명 입력 - 예: 2026학년도 1학기 컴퓨팅 생물학 실습]

본 과제는 컴퓨팅 생물학적 기법을 활용한 진화 분석 파이프라인의 이해를 목적으로 수행되었습니다.
