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

