# Waveguide Mode Theory

광도파로 mode 이론을 평면파부터 2D 단면 도파로까지 단계별로 다루는 웹 강의입니다. 영어/한국어 전환, 수식 (MathJax), 개념 확인 문제, 자동 채점 연습문제와 접어 둔 전체 풀이를 한 페이지에 담았습니다.

A bilingual (English / 한국어) web lecture on optical waveguide mode theory, from plane waves to 2D cross-section waveguides, with concept checks and auto-graded exercises.

- 강의 페이지: `https://<username>.github.io/<repository>/` (GitHub Pages 설정 후 주소)

## 강의 개요

| Section | Parts | 내용 |
|:---|:---|:---|
| 0. Introduction | 1 | 강의 목표, 좌표와 기호 |
| 1. Uniform plane wave | 2–3 | Maxwell 방정식, Helmholtz equation, 평면파의 성질 |
| 2. Fresnel equations | 4–7 | 경계조건과 Snell's law, Fresnel 계수, Brewster angle, 전반사와 evanescent field |
| 3. Planar waveguide | 8–14 | Transverse resonance, TE/TM 분산식, 정규화 b–V 곡선과 그래픽 해법, mode profile과 confinement, radiation mode, group index |
| 4. Multilayer waveguide | 15–19 | Transmission-line (TL) approach, 재귀 반사계수와 ABCD 특성함수, leaky mode와 기판 손실 |
| 5. Numerical method | 20–22 | Bisection, Muller 방법, downhill simplex로 실수·복소 근 찾기 |
| 6. Effective index method | 23–27 | EIM의 원리, channel 도파로와 rib 도파로의 n_eff 계산과 단일모드 조건 |
| 7. Summary | 28 | 정리와 참고 문헌 |

## 연습문제

| Exercise | 내용 | 위치 |
|:---|:---|:---|
| Exercise 1 | 대칭 planar waveguide의 mode 수, n_eff, E-field profile | Part 14 |
| Exercise 2 | 5층 구조의 TE/TM mode와 buffer 두께에 따른 Si 기판 leakage loss | Part 19 |
| Exercise 3 | 매립 channel 도파로의 단일모드 최대 core 굴절률과 그때의 n_eff (EIM) | Part 25 |
| Exercise 4 | Polymer rib 도파로의 단일모드 최대 식각 깊이와 그때의 n_eff (EIM) | Part 27 |

답을 입력하면 바로 채점되고, 각 문제 아래에 단계별 풀이가 접혀 있습니다.

## 기능

- English / 한국어 전환, 밝은 / 어두운 테마
- 왼쪽 목차와 진행 표시 (다음 Part로 넘어가면 완료로 표시)
- 개념 확인 문제와 자동 채점 연습문제
- 진행 상황은 방문자의 브라우저 (localStorage)에만 저장

## 파일

| 파일 | 설명 |
|:---|:---|
| `index.html` | 강의 페이지 전체 (한 파일) |
| `image/` | 그림과 애니메이션 |
| `.nojekyll` | GitHub Pages가 파일을 그대로 제공하도록 하는 빈 파일 |

## GitHub Pages로 배포하기

1. 이 폴더의 파일 전체 (`.nojekyll` 포함)를 저장소의 최상위에 올립니다.
2. 저장소의 **Settings → Pages**에서 Source를 **Deploy from a branch**, Branch를 `main`과 `/ (root)`로 정합니다.
3. 몇 분 뒤 `https://<username>.github.io/<repository>/`에서 강의가 열립니다.

로컬에서 미리 보려면 이 폴더에서 `python -m http.server`를 실행하고 `http://localhost:8000`을 엽니다 (파일을 직접 열면 그림이 보이지 않을 수 있습니다).

## 참고 문헌

- W. H. Hayt, Jr. and J. A. Buck, *Engineering Electromagnetics*, 9th ed., McGraw-Hill (2019).
- K. Okamoto, *Fundamentals of Optical Waveguides*, 3rd ed., Elsevier (2022).
- T. Tamir and S. T. Peng, "Analysis and Design of Grating Couplers," *Applied Physics* **14**, 235–254 (1977).
- H. Kogelnik and V. Ramaswamy, "Scaling rules for thin-film optical waveguides," *Appl. Opt.* **13**, 1857 (1974).
- J. A. Nelder and R. Mead, "A simplex method for function minimization," *Comput. J.* **7**, 308 (1965).
- I. H. Malitson, "Interspecimen comparison of the refractive index of fused silica," *J. Opt. Soc. Am.* **55**, 1205 (1965).
