# MATH SOLVER

<img width="664" alt="스크린샷 2022-03-14 오후 2 04 51" src="https://user-images.githubusercontent.com/59143479/158108801-5c0fcbf1-2120-4ec7-91e8-f8dd0fdc859d.png">

## Intro
Math-Solver는 모두의 연구소의 인공지능 혁신학교 AIFFEL과 자연어처리 스타트업 TUNiB의 협업 프로젝트로 결성된 팀입니다. 2021년도 인공지능 그랜드 챌린지 5차 대회였던 자연어 수학 문제를 파이썬 코드로 풀이를 작성하여 문제를 푸는 테스크를 진행하였습니다. 데이터셋은 지난 대회에 참여한 TUNiB의 레포지토리에 [공개한 데이터](https://github.com/tunib-ai/KMWP)를 사용하였습니다. 후술하는 다양한 실험을 진행하였고, 최종적으로 튜닙이 자체 제작한 테스트셋에서 52%의 Test Accuracy를 달성하였습니다.

## Experiments
### Data Augmentation
- RI(KoEDA)
- Back Translation (ko-en-ko, ko-en-jp-ko)
- 숫자 치환하기(base)

### Model
- koGPT2(base)
- keT5
- Encoder-Decoder (AutoEncoder-AutoRegressive)
- Seq2Tree
- Verifier

## Feedback

### 👍 Good
- Decoder only, Encoder-Decoder(AutoEncoder-AutoRegressive), keT5 등 기존의 모델과 Seq2Tree, Verifer 등 직접 구현한 모델을 사용한 것이 인상적
- 숫자 치환 기법으로 데이터 증강을 시도한 방법도 좋았음

### ☝️ Advice
- skt/ko-gpt-trinity-1.2B 같은 기존보다 더 large-scale model을 사용하였으면 더 좋은 성능이 나왔을 것

## ETC
### PPT
<img width="1179" alt="스크린샷 2022-03-14 오후 2 12 10" src="https://user-images.githubusercontent.com/59143479/158108826-b849f659-6f59-4bf2-a57d-a19012d65b99.png">

[https://docs.google.com/presentation/d/1wk-5zYk-TWuL3NrTKV7mr5ME7hkPYYXyocmmFU4O9UM/edit#slide=id.gf39b8a728b_0_6](https://docs.google.com/presentation/d/1wk-5zYk-TWuL3NrTKV7mr5ME7hkPYYXyocmmFU4O9UM/edit#slide=id.gf39b8a728b_0_6)

### [TUNiB BLOG] TUNiB X AIFFEL DKTC & KMWP 컴피티션 in TUNiB
<img width="989" alt="스크린샷 2022-03-14 오후 2 47 56" src="https://user-images.githubusercontent.com/59143479/158112534-820d11af-d8ab-40c3-84f0-e9363eb0e423.png">

[https://tunib.tistory.com/entry/20220308-TUNiB-x-AIFFEL-DKTC-KMWP-컴피티션](https://tunib.tistory.com/entry/20220308-TUNiB-x-AIFFEL-DKTC-KMWP-%EC%BB%B4%ED%94%BC%ED%8B%B0%EC%85%98)
