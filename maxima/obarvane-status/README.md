![image](https://github.com/user-attachments/assets/e2925549-8783-4099-89e0-ca783aa7ce46)

```
var spans = document.getElementsByTagName('span');
	var l = spans.length;
	for (var i=0;i<l;i++) {
	try {
		if (!spans[i].classList.contains('portlet_nowrap')) continue;
  var tColor;
  if (spans[i].textContent == "QUEUED")continue;
  if (spans[i].textContent == "INPROG")var tColor = "#aa8600";
  if (spans[i].textContent == "PENDING")var tColor = "gray";
		var inspans = spans[i].closest('tr').getElementsByTagName('span');
		var ll = inspans.length;
	for (var ii=0;ii<ll;ii++) {
		inspans[ii].style.color = tColor;
		}
	} catch {}	
	}
``` 
