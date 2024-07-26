![image](https://github.com/user-attachments/assets/e2925549-8783-4099-89e0-ca783aa7ce46)

potrebno je odstraniti komentarje oz. prilagoditi po želji.

```
var spans = document.getElementsByTagName('span');
	var l = spans.length;
	for (var i=0;i<l;i++) {
	try {
		if (!spans[i].classList.contains('portlet_nowrap')) continue;
    var tColor = '';
  if (spans[i].textContent == "INPROG") tColor = "#aa8600";
  if (spans[i].textContent == "PENDING") tColor = "gray";
  if (tColor == '')continue;
		var inspans = spans[i].closest('tr').getElementsByTagName('span');
		var ll = inspans.length;
	for (var ii=0;ii<ll;ii++) {
		//inspans[ii].style.color = tColor;
		//inspans[ii].style.textDecorationLine = 'line-through';
		}
tColor = '';
	} catch {}	
	}
``` 
