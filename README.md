# Popcat-Click-Auto-Clicker

## HOW TO USE?
1. Open the [Website](https://popcat.click)
2. Open Inspect Element Tab (Click F12)
3. Click on Console
4. Insert code bellow and run (Click Enter)
 
```
var event = new KeyboardEvent('keydown', {
	key: 'g',
	ctrlKey: true
});

setInterval(function(){
	for (i = 0; i < 100; i++) {
		document.dispatchEvent(event);
	}
}, 100); 
```

> Interval 100 because will not detected as bot. 
> (If cat's eyes turn red means detected as bot and points will not be counted) 
### What happens if you put interval as 0 :
![Untitled](https://user-images.githubusercontent.com/66457844/129150335-6b8522a6-17b4-45ff-bf58-20139883260d.png)
