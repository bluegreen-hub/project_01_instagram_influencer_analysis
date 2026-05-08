# Instagram Influencer Analysis

This project performs exploratory data analysis and preprocessing on Instagram influencer data, and presents the results in a Tableau dashboard.

## Project Structure
- `notebooks/`: Contains the Jupyter notebook for data preprocessing and EDA.
- `data/processed/`: Contains the processed data ready for Tableau.
- `dashboard/`: Contains the link to the Tableau Public dashboard.
- `assets/`: Contains images such as the dashboard thumbnail.

## 📊 데이터 분석 인사이트 (EDA Insights)

Jupyter Notebook을 통한 탐색적 데이터 분석(EDA) 결과, 인플루언서의 영향력(Influence Score)을 결정하는 요인에 대해 다음과 같은 주요 인사이트를 도출했습니다.

### 1. 영향력 점수(Influence Score)의 주요 결정 요인
* **압도적인 요인**: 인플루언서의 영향력 점수는 **'팔로워 수(Followers)'**가 압도적인 영향을 미칩니다. (팔로워 수와 누적 좋아요 수는 강한 양의 상관관계를 가짐)
* **보조적 요인**: 팔로워 수 다음으로는 **참여율(Engagement Rate)**, **누적 좋아요 수(Total Likes)**, **최근 60일 참여율** 등이 영향력 점수에 보조적으로 작용합니다.
* **낮은 연관성**: 반면, '신규 게시물 평균 좋아요 수'나 '평균 좋아요 수' 자체만으로는 영향력 점수를 온전히 설명하기 어렵습니다. 다른 지표들은 영향력 점수와 크게 연관성이 없는 것으로 나타났습니다.

### 2. 예외 케이스 및 추가 발견 사항
* **비활성 거대 계정**: 팔로워 수는 매우 많지만 반응(Engagement)은 현저히 적은 계정들이 존재합니다.
* **작지만 강한 계정**: 팔로워 수는 상대적으로 적음에도 불구하고 높은 인플루언서 스코어를 기록하는 이례적인 계정들이 존재합니다. 이는 팔로워 수가 무조건적으로 영향력 점수와 100% 일치하지는 않음을 보여주며, 높은 참여율 등 다른 숨은 요인이 작용함을 암시합니다.

## 📈 대시보드 (Tableau Dashboard)

[![내가 분석한 인플루언서 지표](https://public.tableau.com/static/images/3_/3_17781236906790/sheet12/1.png)](https://public.tableau.com/views/3_17781236906790/sheet12?:language=ko-KR&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

*이미지를 클릭하면 태블로 퍼블릭(Tableau Public) 대시보드로 이동합니다.*
