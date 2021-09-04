#  LED Board

## 기능
- 원하는 글씨를 다양한 색상을 선택해서 보여준다

## 활용 기술
- Storyboard
    - AutoLayout
    - stack view
    - Alpha
- Navigation Controller
    - 화면 전환 및 데이터 전달
- Assets
-UITextField

---

### Stack View
- label, button 등 여러가지를 하나로 묶을 때
- 가로 stack view, 세로 stack view

### Assets
- 이미지나 색상, 음원 파일 등 필요한 리소스들을 담아두는 곳
- 1x, 2x, 3x : 기기별로 사이즈가 다르므로 그것에 맞는 이미지를 자동으로 적용한다

### 색상 변경시 Alpha 값 변경
- 삼항연산자 (`조건식 ? <true이면 실행할 구문> : <false이면 실행할 구문>`)

``` swift
private func changeTextColor(color: UIColor) {
    // (주어진 color가 .yellow라면 0.2, 아니면 1)를 yellowButton의 alpha값으로 지정
    self.yellowButton.alpha = color == UIColor.yellow ? 0.2 : 1
}
```

### [데이터 전달](https://github.com/prettyturtle/ScreenTransitionExample)
