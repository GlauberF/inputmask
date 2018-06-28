# inputmask
Mask baseada no Input Mask plugin


HTML
```
<input id="aplica_format_tel"/>
```

JS
```
$(document).ready(function(){
    $("#aplica_format_tel").inputmask("phone", { onUnMask: function(maskedValue, unmaskedValue) {
        console.log(maskedValue)
        console.log(unmaskedValue)
        return unmaskedValue;
      }});
    $('#aplica_format_tel').inputmask({ 'autoUnmask' : true});
});
```
