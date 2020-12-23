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
