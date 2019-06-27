#자료형
-기본 자료형 (Primitive) 인 여섯 가지 데이터 형
 -부울
 -없는
 -정의되지 않음
 -번호
 -끈
 -기호 (ECMAScript 6에 추가됨)
 -별도로 객체 도 있음
js 제어 할 태그 지정하기
<body style="background-color:black;"> 
	<h1><a herf="index.html">WEB</a></h1>
    <input type="button" value="night" onclic="
		document.querySelector('body').style.backgroundColor = "black";
		document.querySelector('body').style.color = "white";
		//selector은 css의 selector
    ">
    <input type="button" value="day" onclic="
    	document.querySelector('body').style.backgroundColor = "white";
    	document.querySelector('body').style.color = "black";
    ">
</body>    
조건문
운영자

"A === B": 비교 연산자. 거짓 값 false
"A <B"
<body> 
	<h1><a herf="index.html">WEB</a></h1>
    <input id="night_day";type="button" value="night" onclick="
    if (document.querySelecctor(#night_day).value === 'night') {
    	document.querySelector(#night_day).value = 'day';
		document.querySelector('body').style.backgroundColor = "black";
		document.querySelector('body').style.color = "white";
		}
	else {
	    document.querySelector(#night_day).value = 'night';
    	document.querySelector('body').style.backgroundColor = "white";
    	document.querySelector('body').style.color = "black";
    	}
    ">
</body>    
리팩토링 (리팩토링)
비공식적이고 비경제적인 부분을 활용하면 편재하고 중복성을 유지할 수있다.

<body> 
	<h1><a herf="index.html">WEB</a></h1>
    <input type="button" value="night" onclick="
    var target = document.querySelector('body');
        if (this.value === 'night') {
            this.value = 'day';
            target.style.backgroundColor = "black";
            target.style.color = "white";
            }
        else {
            this.value = 'night';
            target.style.backgroundColor = "white";
            target.style.color = "black";
            }
        ">
</body>    
배열
<script>
	var array = ["one","two"];
</script>
<h2>get</h2>
    <script>
      document.write(array[0]);
      document.write(array[1]);
    </script>
<h2>add</h2>
    <script>
      coworkers.push('duru');
      coworkers.push('taeho');
    </script>
<h2>count</h2>
    <script>
      array.write(coworkers.length);
    </script>
repeat
<body>
	<h1>Loop</h1>
	<script>
		document.write('<li>1<li>');
		var i = 0;
		while(i < 3){
			document.write('<li>1<li>');
			document.write('<li>1<li>');
			document.write('<li>1<li>');
			i++;
		}
	</script>
</body>
배열 및 반복문 (루프 및 배열)
<body>
	<h1>Loop & Array</h1>
	<script>
		var array = ["one","two",'three'  ];
	</script>
	<script>
        var i = 0;
        while(i < coworkers.length){
          document.write('<li><a href="http://a.com/'+coworkers[i]+'">'+coworkers[i]+'</a></li>');
          i = i + 1;
        }
    </script>
</body>
combined repeat application
<body> 
	<h1><a herf="index.html">WEB</a></h1>
    <input type="button" value="night" onclick="
    var target = document.querySelector('body');
        if (this.value === 'night') {
            this.value = 'day';
            target.style.backgroundColor = "black";
            target.style.color = "white";
            var i = 0;
        	while(i < alist.length){
            alist[i].style.color = 'powderblue';
            i = i + 1;
          }
            }
        else {
            this.value = 'night';
            target.style.backgroundColor = "white";
            target.style.color = "black";
            var i = 0;
        	while(i < alist.length){
            alist[i].style.color = 'blue';
            i = i + 1;
          }
      ">
</body>    
함수
<script>
	function sum(num1, num2) {
        return num1+num2;
	}
	document.write('<div style="color:red">' + sum(3,4)'</div>');
</script>

<script>
nightHandler(self)
    var target = document.querySelector('body');
    	if (self.value === 'night') {
            self.value = 'day';
            target.style.backgroundColor = "black";
            target.style.color = "white";
            var i = 0;
            while(i < alist.length){
            alist[i].style.color = 'powderblue';
            i = i + 1;
              }
                }
        else {
        	self.value = 'night';
            target.style.backgroundColor = "white";
            target.style.color = "black";
            var i = 0;
            while(i < alist.length){
            alist[i].style.color = 'blue';
                i = i + 1;
        }	
    ">
</script>
<body> 
	<h1><a herf="index.html">WEB</a></h1>
    <input type="button" value="night" onclick="
    	nightHandler(this)"
</body>    
