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
![Untitled](https://user-images.githubusercontent.com/66457844/129151245-231af8fa-aa24-4f40-a52f-c130aa77b71c.png)

## Still getting detected as bot? Use a different browser and try this:
```
var event = new KeyboardEvent('keydown', {
	key: 'g',
	ctrlKey: true
});

setInterval(function(){
	for (i = 0; i < 1; i++) {
		document.dispatchEvent(event);
	}
}, 100); 
```
> This code will click only once per 100 milliseconds. 

## A simpler code that also works:
```
setInterval(()=>{document.dispatchEvent(new Event("keydown"))},40)
```
