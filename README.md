# play-ground-css

# 가상 선택자 
    presudo.html
        hover
        active
        visited
        focus

# 가상 클래스 선택자
    presudoSeletor.html
        ul li:first-child {
            background-color: lightgreen;
        }
        ul > li:last-child {
            background-color: yellowgreen;
        }

# NTH OF TYPE 
    nthOfType.html
		a. p:nth-of-type(1)  p 태그중 첫번째
		b. 태그 선택용으로만 사용 

# 가상 요소 선택자 
    before.html  after.html
        가상 요소 선택자 작성시 반드시 :: 두개 (작동 안하는것은 아니지만 :: 두개 작성 한다.)
        :+1:

# 속성 선택자 
    attr.html  attr_carot.html  :arrow_left:
 		a. [target] { text-decortion:none; }
		b. [target="_blank] { color : blue; }
		d. [class^="btn"] { list-style : none ; } 속성값이 btn로 시작하는
        d. [class$="success"] { list-style : none ; } 속성값이 success로 끝나는

# CSS Reset 
    <!-- CSS 리셋 코드  -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.css" />
# CSS float
    float : left, right
    clear : left, right, both
    clearfix::after{
        content:"";
        clear:both;
        display:block;
    }
    
# CSS position 
    position: relative
    position: absolute
    position: fixed
    position: sticky
    position: static 
        top:50px 
        left:
        right:
        bottom: 
    부모 
    position:relative
    자식
    z-index:1...n 높은 순서가 우선 으로 쌓임.

# CSS overflow
    overflow : auto
    overflow : hidden
    overflow : scroll
    overflow : none

# CSS background
    background-image: url("")
    background-image: url(""), url("")  //다중 이미지 배치 가능 
    background-position: left center; %, px, em
    background-repeate: no-repeat, repeat-x, repeat-y, repeat
    background-size: auto 100%, 100px, contain, cover
    background-color: tomato
    background-attachment : scroll, fixed, local

# CSS transition 
    transition-propert          전환 효과를 사용할 속성 이름.       all
    transition-duration         전환 효과의 지속시간 설정           0s
    transition-timeing-function 타이밍 함수 지정(타이밍 함수란)     ease
    transition-delay            전환효과의 대기시간 설정            0s

    transition-timeing-function 
        ease
        ease-in 
        ease-out
        steps(3)

# CSS Transform
    transform       요소의 변환 효과(변형)을 지정 
    transform: rotate(20deg) translate(10px, 0) -> translate 는 이동 개념 x, y 축입니다. 
    transform: translate(10px, 20px); 이동 x축 10px , y축 20px
    transform: rotate(30deg); 절대값으로 회전축 셋팅
    transform: skew(20px, 30px); 비틀기 x 축 y축 -값도 먹음 
    함께 사용 
    transform: rotate(30deg) translate(10px, 20px);

# CSS Transform 3d
    translate3d(x,y,z)  이동 x,y,z 축 
    perspective 는 가장 앞에 선언되어야함 
    transform: perspective(130px) rotateY(10deg); //rotateX(10deg) 

# CSS Transform 변환속성
    transform-origin    요소의 변환의 기준점을 설정
    transform-style     3D 변환 요소의 자식 요소도 3D 변환을 사용할지 설정
    perspective         하위 요소를 관찰하는 원근 거리를 설정
    perspective-origin  원근 거리의 기준점을 설정 
    backface-visiblility  3D 변환으로 회전된 요소의 뒷면 숨김을 설정 

    transform-origin , left,right,center,% 단위 
    
# CSS card example code


# CSS Animation 
    아래와 같이 세팅함. 
    .box{
        animation: first-animation 2s;
    }
    @keyframes first-animaition { 
        0% { width: 100px}
        100% { width: 200px}
    }
    개별 속성
        animation-name : @keyframes 에 이름 지정 
        animation-duration: 3s 
        animation-timing-function: ease, linear
        animation-delay : 3s 
        animation-iteration-count : 3,infinity
        animation-direction: reverse, alternate 
        animation-fill-mode: none, forwards, backwards, both  
        animation-play-state : paused, running 
    
    단축 속성 
        이름, duration, 반복, 방향, delay, timing function 
        animation: move 1s infinity alternate 1s linear 
        
# FLEX 속성
    display:flex
    display:inline-flex 

    Container 
        flex-flow : 방향 wrap
            flex-direction : row , column , -reverse
            flex-wrap : nowrap, wrap , -reverse
        
        justify-content : flex-start, flex-end, center, space-between, space-around
        align-content : stretch, flex-start, flex-end, center, space-between, space-around   (랩 으로 떨어져야 먹음, 단체로 먹임)
        align-items : baseline stretch, flex-start, flex-end, center (랩으로 떨어져야 먹고,아이템축별로 먹임 교차축)
    Item
        flex : grow shrink basis -> 1 로 설정시 (0 1 0) 세팅 됨.
            flex-grow : 1 -> 합산에 분할만큼 커짐 , 여백을 나눠 가지는 개념임. basis 를 0으로 하면 그대로 먹음
            flex-shrink : 1 -> 합산에 분할만큼 작아짐  , 여백을 나눠 가지는 개념임. basis 를 0으로 하면 그대로 먹음
            flex-basis : 기본값 auto , 0 , 혹은 기본 100px 이렇게 줄수 있음.
        
        align-self : auto , stretch , flex-start , flex-end, center , baseline
            item 개별로 위치 지정시 사용 

    





























