# Data visualization with Leaflet (11-13 Jul 2018)

### Resource
 - https://leafletjs.com/
- https://drive.google.com/drive/folders/1T4eovBVE7xt0w32cTw7qP07Z9d7-nO6z
- https://docs.google.com/document/d/1csqmVG97knOOLjy1qcdPyqHYOF-fViCanDSZCe4z6kk

### Editor (recommend)
[Visual Studio Code](https://code.visualstudio.com/)

### VScode Extention (recommend)
- [Live Server] เป็นตัวช่วยในการรันไฟล์ html และ javascript
- [HTML Snippets] เป็นตัวช่วยในการสร้าง code HTML
- [Code Outline] เป็นตัวช่วยในการดู Code ให้ง่ายขึ้น
- [jQuery Code Snippets] เป็นตัวช่วยในการสร้าง code jquery

### Start!!
#### เริ่มต้นที่ basic map
- สร้างหน้า html

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Basic map!</title>
</head>
<body>   
</body>  
</html>
```
- สร้าง map อย่างง่ายกัน เพิ่ม css กำหนดความสูง ความกว้าง
```css
        #mapid{
            height: 100vh;
            width: 100vh;
        }
```
- สร้าง script เพื่อแสดง  map
```js
var mymap = L.map('mapid').setView([13.753256, 100.500082], 5);
        
        L.tileLayer('https://api.tiles.mapbox.com/v4/{id}/{z}/{x}/{y}.png?access_token=pk.eyJ1IjoibWFwYm94IiwiYSI6ImNpejY4NXVycTA2emYycXBndHRqcmZ3N3gifQ.rJcFIG214AriISLbB6B5aw', {
            maxZoom: 18,
            attribution: 'Map data &copy; <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors, ' +
                '<a href="https://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>, ' +
                'Imagery © <a href="https://www.mapbox.com/">Mapbox</a>',
            id: 'mapbox.streets'
        }).addTo(mymap);
```
- เพิ่ม ส่วนแสดงผลใน html
```html
<div class="" id="mapid"></div>
```





[jQuery Code Snippets]:https://marketplace.visualstudio.com/items?itemName=donjayamanne.jquerysnippets


[Code Outline]:https://marketplace.visualstudio.com/items?itemName=patrys.vscode-code-outline

[HTML Snippets]:https://marketplace.visualstudio.com/items?itemName=abusaidm.html-snippets

[Live Server]:https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer