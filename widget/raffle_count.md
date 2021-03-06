# 2. 이벤트 응모자수 표시

### 소개

특정 이벤트에 응모자가 몇명인지를 표시합니다.\
이벤트 페이지 등에 응모자수를 표시하여 래플 이벤트의 신뢰성을 높일 수 있습니다.

### 미리보기

| Default Style                           | Blank Style                             |
| --------------------------------------- | --------------------------------------- |
| ![](<../.gitbook/assets/image (2).png>) | ![](<../.gitbook/assets/image (3).png>) |

### 사용방법

응모내역을 표시하고 싶으신 페이지에 아래와 같은 코드를 추가만으로\
간편하게 사용하실 수 있습니다.\


default style

```markup
<div class="__raffle_count_wrap__" wrap-style="default" event_no="">
    응모자수 확인중입니다.
</div>
```



blank style

```markup
<div class="__raffle_count_wrap__" wrap-style="blank" event_no="">
    응모자수 확인중입니다.
</div>
```



event\_no 옵션을 사용할 경

```markup
<div class="__raffle_count_wrap__" wrap-style="blank" event_no="102">
    응모자수 확인중입니다.
</div>
```





#### 사용가능한 옵션&#x20;

| 옵션명        | 소개                                                                                                                                                                                                                                                       |
| ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| wrap-style | <p><strong>(필수항목아님)</strong><br>사용하고자 하는 스타일을 지정합니다</p><p>스타일은 현재 'default'와 'blank'를 사용하실 수 있으며,<br></p><p>'default'를 사용시 기본적인 css를 통해 간단한 디자인이 자동 적용되고,<br></p><p>'blank'를 사용시 css가 적용되지 않은 형태로 반환됩니다.<br><br>지정하지 않으실 경우 자동으로 'blank' 스타일이 적용됩니다.</p> |
| event\_no  | <p><strong>(필수항목아님)</strong><br><strong></strong>특정 이벤트에 대한 응모자수만 표시하고 싶을 때 사용합니다.<br></p><p>이벤트의 고유번호를 입력해주시면 되며,<br>이벤트 고유번호는 래플 관리자 페이지 > 이벤트 수정에서 확인하실 수 있습니다.<br><br>입력하지 않으실 경우 모든 이벤트에 대한 누적 응모자수가 표시됩니다.</p>                                     |
