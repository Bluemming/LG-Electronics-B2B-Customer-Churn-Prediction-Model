<h4 align='center'> LG Aimers 4기 (LG전자) </h4>

<h1 align='center'> MQL 데이터 기반 B2B 영업기회 창출 예측 모델 개발 </h1>

&nbsp;  

<br>   
<div align='center'>
<table>
    <thead>
        <tr>
            <th colspan="4"> 팀 구성원 </th>
        </tr>
    </thead>
    <tbody>
        <tr>
          <tr>
            <td align='center'><a href="https://github.com/mixk0n9"><img src="https://github.com/mixk0n9.png" width="100" height="100"></td>
            <td align='center'><a href="https://github.com/ymk713"><img src="https://github.com/ymk713.png" width="100" height="100"></td>
            <td align='center'><a href="https://github.com/Bluemming"><img src="https://github.com/Bluemming.png" width="100" height="100"></td>
            <td align='center'><a href="https://github.com/iwantpubao"><img src="https://github.com/iwantpubao.png" width="100" height="100"></td>
          <tr>
            <td align='center'>김민경</td>
            <td align='center'>김유미</td>
            <td align='center'>민지현</td>
            <td align='center'>성현수</td>
          </tr>
        </tr>
    </tbody>
</table>
</div>

<h3 align='center'> 온라인 해커톤 8위, 오프라인 해커톤 9위 달성 </h3>

<h4 align='center'> <a href="https://www.lgresearch.ai/news/view?seq=421"> AI 전문가의 길을 열어주는 LG Aimers 4기 과정 마무리</a>
 </h4>

&nbsp;  

## 기간
2024.01.02 - 2024.04.07

## 목표
- LG전자의 B2B 영업 성공 기회를 예측하는 모델 개발
- B2B 마케팅에 유의미한 영향을 주는 요인을 파악하여 솔루션 제시
- 데이터 불균형 문제 해결, 예측 모델 성능 향상

&nbsp;  

## 사용 데이터
LG전자 MQL 데이터(B2B)
- 텍스트 변수가 과반수
- 타겟 레이블이 불균형

&nbsp;  

## 분석 방법
- 파생 변수 생성
  1. 동일 기업과 동일 거래자가 계약을 체결한 횟수
  2. LG전자 기준의 제품 대분류, 중분류 카테고리
  3. 사업 분류(비공개)로 산출된 수치 데이터를 역으로 이용하여 사업 분류 카테고리로 사용
- 범주형 변수 처리에 효과적인 CatBoost모델을 사용
- class_weights변수로 불균형 고려

&nbsp;  

## 결과
- 계약자ID 관련 변수가 매우 큰 중요도
- oversampling(과대표집)이 불가한 상황에서 class_weights부여가 성능 향상에 큰 기여

&nbsp;  

## 분석 과정

