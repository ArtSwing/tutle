# tutle
tutle Project
//20200804
오늘 서울의 날씨는 먹구름이 많고 가끔 소나기가 내린다
문장 입력
	ㄴsplit 띄어쓰기
	오늘/서울의/날씨는/먹구름이/많고/가끔/소나기가/내린다.
		ㄴsplit 접두사 접미사(형태소구분#나중)
		오늘/서울:의/날씨:는/먹구름:이/많:고/가끔/소나기:가/내린:다.
			ㄴ추출
			오늘/서울/날씨/먹구름/많/가끔/소나기/내린
			null  /   의/   는/       이/고/ null/       가/    다
null일경우 붙여줌 ?
	ex)오늘서울/날씨/먹구름/많/가끔소나기/내린
		의/   는/       이/고/             가/   다
관형격조사일경우 붙여줌 ?
	ex)오늘서울의날씨/먹구름/많/가끔소나기/내린
		         는/       이/고/              가/   다
	how : 의

주제인 보조사 : 오늘서울의 날씨
	how : 는

문장 나누기 : 먹구름/많	가끔소나기/내린
	            이/고                       가/   다
            how : 고
            after : 고 -> 다

주어 : 먹구름	가끔소나기
how :        이                       가

서술어 : 많	내린
how :     다                다

찾을 내용 :	1.오늘서울의날씨는먹구름이많다.
		2.오늘서울의날씨는가끔소나기가내린다.

//20200805
@한글
1.음운
	ㄴ말의 뜻을 구별해주는 소리의 가장 작은 단위
	ㄴ1)음소
		ㄴ음소는 더이상 작게 나눌 수 없는 음운론상의 최소 단위
		ㄴ자음과 모음
		ㄴex)밥 -> ㅂ/ㅏ/ㅂ
	ㄴ2)운소
		ㄴ단어의 의미를 분화하는데 관여하는 음소 이외의 운율적 특징
		ㄴ높낮이, 길이, 세기 등
2.음절
	ㄴ하나의 종합된 음의 느낌을 주는 말소리의 단위
	ㄴex)밥을 먹는다 -> 바/블/멍/는/다
3.###################################################형태소###################################################
	ㄴ뜻을 가진 가장 작은 단위
	ㄴex)몇 개의 문장을 통해 형태소 분석을 해 보겠습니다.
		ㄴ실질형태소 : 몇         /개               /문장  /통     /형태  /소     /분석  /하-             /보-
			        [관형사] [(의존) 명사] [명사] [어근] [명사] [명사] [명사] [동사의어근] [동사의어근]
		ㄴ형식형태소 : 의       /을     /-하-(다)/-여           /을     /-여          /-겠-             /-습니다
			        [조사] [조사] [접미사] [어말어미] [조사] [어말어미] [선어말어미] [어말어미]
		ㄴ자립형태소 : 몇          /개              /문장  /형태  /소     /분석
			        [관형사] [(의존) 명사] [명사] [명사] [명사] [명사]
		ㄴ의존형태소 : 의       /을     /통     /-하-(다) /-여          /을     /하-              /-여         /보-              /-겠-            /-습니다
			        [조사] [조사] [어근] [접미사] [어말어미] [조사] [동사의어근] [어말어미] [동사의어근] [선어말어미] [어말어미]
	ㄴ1)실질형태소
		ㄴ어휘적의미를 가진 가장 작은 말의 단위
		ㄴ어휘형태소 라고도 함
		ㄴ어근을말함
			ㄴ9품사중 조사를 제외한 명사, 대명사, 수사, 관형사, 부사, 동사, 형용사, 감탄사
			ㄴ단어를 분석할때 실절적 의미를 나타내는 중심이 되는 부분
			ㄴex)샛노랗다 -> 노랗-
			ㄴ어근과 어간의 차이
				ㄴex)샛노랗다 -> 어근 : 노랗- / 어간 : 샛노랗-
	ㄴ2)형식형태소
		ㄴ문법적 의미를 가진 가장 작은 말의 단위
		ㄴ문법형태소 라고도 함
		ㄴ접사, 어미, 조사
			ㄴ(1)접사
				ㄴ단독으로 쓰이지 아니하고 항상 다른 어근이나 단어에 붙어 새로운 단어를 구성하는 부분
				ㄴ접두사, 접미사
				ㄴex)샛노랗다 -> 샛-
			ㄴ(2)어미
				ㄴ용언 및 서술격 조사가 활용하여 변하는 부분
				ㄴex)샛노랗다 -> -다
				ㄴ어말 어미, 선어말 어미
	ㄴ3)자립형태소
		ㄴ다른말에 의존하지 아니하고 혼사 설 수 있는 형태소
		ㄴ형식 형태소와의 차이는 동사의 어근, 형용사의 어근은 포함X
	ㄴ4)의존형태소
		ㄴ다른말에 의존하여 쓰이는 형태소
		ㄴ어간, 어미, 접사, 조사 따위
	ㄴ5)형태소의 이형태
		ㄴ(1)음운론적 이형태
			ㄴ주격조사 이, 가
				ㄴ명사의 마지막 받침 O : 이
				ㄴ받침 X : 가
		ㄴ(2)형태론적 이형태
			ㄴ어간의 마지막 모음 ㅏ, ㅗ O : -아서
			ㄴ모음 ㅏ, ㅗ X : -어서
			ㄴ모음 하- : -여
			
#########################################################################################################
4.단어
	ㄴ분리하여 자립적으로 쓸 수 있는 말이나 이에 준하는 말
	ㄴ9품사
		ㄴ1)명사
			ㄴ사물의 이름을 나타내는 단어
		ㄴ2)대명사
			ㄴ명사를 대신하는 단어
		ㄴ3)수사
			ㄴ수량이나 순서를 나타내는 단어
		ㄴ4)관형사
			ㄴ명사, 대명사, 수사를 꾸며 주는 단어
		ㄴ5)부사
			ㄴ동사, 대명사, 문장을 더 분명하게 꾸며주는 단어
		ㄴ7)조사
			ㄴ문법적 관계를 표시하거나 그 말뜻을 도와주는 단어
		ㄴ7)동사
			ㄴ움직임을 나타내는 단어
		ㄴ8)형용사
			ㄴ상태를 나타내는 단어
		ㄴ9)감탄사
			ㄴ놀람, 느낌, 부름, 응답을 나타내는 단어
	ㄴ기능
		ㄴ1)체언
			ㄴ문장에서 주어의 기능을 할 수 있는 단어
				ㄴ명사, 대명사 , 수사
		ㄴ2)관계언
			ㄴ문장에서 단어들의 관계를 나타내는 단어
				ㄴ조사
		ㄴ3)수식언
			ㄴ뒤에 오는 말을 꾸며 주는 단어
				ㄴ관형사, 부사
		ㄴ4)용언
			ㄴ문장에서 서술어의 기능을 하는 단어
				ㄴ동사, 형용사
		ㄴ5)독립언
			ㄴ독립적으로 사용할 수 있는 단어
				ㄴ감탄사
5.어절
	ㄴ문장을 구성하고 있는 각각의 마디
	ㄴ띄어쓰기의 단위가 됨
	ㄴex)철수가 집에서 음악을 듣는다 -> 철수가/집에서/음악을/듣는다
6.구절
	ㄴ구와 절을 아울러 이르는말
	ㄴ1)구
		ㄴ문장 내에서 두 개 이상의 단어로 이루어져 주어와 술어 관계가 없는 덩어리
		ㄴ명사구, 동사구, 형용사구, 관형사구, 부사구
		ㄴex)저기 사진을 찍는 사람이 내 친구야. -> 저기 사진을
			ㄴ2개의 단어로 이루어짐, 주어 서술어는 아님
	ㄴ2)절
		ㄴ주어와 서술어 관계가 이루어진 말
		ㄴ관형절, 명사절, 부사절, 인용절, 서술절
		ㄴex)날씨가 좋으니 기분도 좋다 -> 날씨가 좋으니 / 기분도 좋다
			ㄴ2개의 어절이 합쳐졌고 좋다라는 형용사가 주어 서술어의 관계
7.문장
	ㄴ생각이나 감정을 말로 표현할 때 완결된 내용으로 나타내는 최소 단위
	ㄴ특징으로는 마침표 느낌표 물음표가 들어감
8.문단
	ㄴ여러 문장이 모여 하나의 중심 생각을 나타내는 덩어리
