# A-calculator-App
make some calculator App<br>
<br>
## 활용 기술
UIStackView<br>
IBDesignables<br>
IBInspectable<br>
<br>
## UIStackView
열 또는 행에 View들의 묶음을 배치할 수 있는 간소화된 인터페이스<br>
스택뷰를 사용하면 오토레이아웃을 많이 사용하지 않아도 쉽게 UI 구성이 가능하다<br>
위치와 구성에 따라 Vertical Stack View 와 Horizontal Stack View를 사용하여 구성한다<br>
# Stack View에는 다양한 속성이 있다.
Asis : 스택 뷰의 방향을 결정, vertical로 설정하면 스택뷰가 가로 방향으로 추가되고, horizontal로 추가하면 세로 방향의 스택 뷰가 추가된다<br>
## Alignment : 스택 뷰의 서브 뷰들을 어떤식으로 정렬할지 결정하는 속성
-스택뷰의 방향이 Horizontal 일 경우 아래 위 공간을 전부 채우기 위해 서브 뷰들을 늘리고 vertical인 경우는 좌우 공간을 전부 채우기 위해 서브 뷰들을 늘린다.<br>
-Leading: Vertical 스택 뷰에서 서브뷰들이 스택 뷰의 리딩에 맞춰 정렬이 된다(왼쪽 정렬)<br>
-Top : 스택뷰의 위쪽으로 정렬<br>
-First Baseline: 서브 뷰들의 first baseline에 맞춰 서브 뷰들이 정렬된다. 이 옵션은 오직 horizontal 스택 뷰에서만 사용할 수 있다.<br>
-center: 서브 뷰들의 센터를 스택뷰의 센터에 맞춰 정렬한다.<br>
-Trailing: 스택 뷰의 오른쪽에 맞춰 서브 뷰들을 정렬한다.<br>
-Bottom: Horizontal 스택 뷰에서 스택 뷰의 아래쪽에 맞추어 정렬한다<br>
-Last Baseline: horizontal 스택 뷰에서 서브 뷰들의 Last Baseline에 맞추어 정렬하는 속성<br>
## Distribution : StackView안에 들어가는 뷰들의 사이즈를 어떻게 분배할지 설정하는 속성
-Fill : 스택 뷰의 빈공간을 꽉꽉 채우기 위해, 알아서 서브 뷰들을 조정 (compression registancy를 비교)<br>
-Fill Equally : 서브 뷰들의 가로 길이가 같도록 채운다<br>
-Fill Proportionally : 스택뷰의 방향에 따라 서브뷰가 갖고 있던 크기에 비례해 공간을 차지하도록 만들어진다<br>
-Equal Spacing : 서브 뷰 사이의 간격이 균등하도록 배치한다.<br>
-Equal Centering : 서브 뷰의 방향에 따라 서브 뷰들의 센터와 센터 간격이 동일하도록 맞춘다.<br>
<br>
## Spacing
스택 뷰 안에 들어가는 뷰들의 간격을 조정하는 속성<br>
spacing 값에 따라 서브 뷰들의 간격이 넓어지거나 좁아진다 <br>
