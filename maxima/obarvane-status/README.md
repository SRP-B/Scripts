![image](https://github.com/user-attachments/assets/e2925549-8783-4099-89e0-ca783aa7ce46)

potrebno je odstraniti komentarje oz. prilagoditi po želji.

```
var bugg= document.getElementById('csjRan');
if (bugg != null) bugg.style.display = 'none';

var runOnSpans = function(element, eCallback) {
var inspans = element.closest('tr').getElementsByTagName('span');
for (var ii=0;ii<inspans.length;ii++) {eCallback(inspans[ii]);}
}
	var spans = document.getElementsByTagName('span');
	var l = spans.length;
	for (var i=0;i<l;i++) {
	try {
		if (!spans[i].classList.contains('portlet_nowrap')) continue;

  if (spans[i].textContent == "INPROG"){
  //runOnSpans(spans[i], (el) => el.style.textDecorationLine = 'line-through');
  //runOnSpans(spans[i], (el) => el.style.color = '#aa8600');
  }
  if (spans[i].textContent == "PENDING") {
  //runOnSpans(spans[i], (el) => el.style.textDecorationLine = 'line-through');
  //runOnSpans(spans[i], (el) => el.style.color = 'gray');
  }
  if (spans[i].textContent.startsWith('FURS')) {
  //runOnSpans(spans[i], (el) => el.style.textDecorationLine = 'line-through');
  //runOnSpans(spans[i], (el) => el.style.color = 'gray');
  }
	} catch {}	
	}
``` 
