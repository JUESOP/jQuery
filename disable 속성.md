회원가입을 할때 중복아이디를 입력할 경우 button 클릭을 하기전에 ajax를 이용하여 미리 중복검사를 한 뒤
중복인지 아닌지를 확인 해주는 코드를 작성하고 싶었습니다. 

 
### 그리고 유저 생성 버튼을 disabled 속성으로 막아 회원가입을 못하도록 설계하려 했습니다.




```
<input type="submit" id="button_joinus" value="가입하기" disabled="">
```
<위와 같은 버튼이 있다고 가정해보자>

  





## javascript에서 disabled라는 함수를 사용할 수 있습니다.
```
<script>
    var button_joinus = document.getElementById('button');
    #button_joinus 변수를 이용해서 html의 버튼을 선언합니다.
 
    button_joinus.disabled = true;
</script>
```




## 참고로 jQuery를 이용하면 attr함수를 이용하여 해결 할 수 있습니다.
```
$button_joinus = $('.button_joinus').attr('disabled', true);
$button_joinus = $('.button_joinus').attr('disabled', false);
```


출처: https://paphopu.tistory.com/entry/Javascript-jQuery를-이용해-button에-disable-속성-해제-적용 [jadehan]
