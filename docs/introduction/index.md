<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>3D 賽車遊戲</title>
    <script src="https://aframe.io/releases/1.2.0/aframe.min.js"></script>
    <style>
        body { margin: 0; overflow: hidden; }
        a-scene { height: 100vh; }
    </style>
</head>
<body>

<!-- A-Frame 场景 -->
<a-scene>
    <!-- 創建賽車 -->
    <a-box position="0 0.5 -3" rotation="0 0 0" color="#4CC3D9" width="1" height="0.5" depth="2"></a-box>
    
    <!-- 增加控制按鍵 -->
    <a-entity position="0 1.5 -4" camera look-controls>
        <a-cursor></a-cursor>
    </a-entity>

    <!-- 地面 -->
    <a-plane position="0 0 -10" rotation="-90 0 0" width="500" height="500" color="#7BC8A4"></a-plane>
    
    <!-- 增加障礙物 -->
    <a-box position="0 0.5 -10" color="#ff0000" width="2" height="2" depth="2"></a-box>
    <a-box position="3 0.5 -15" color="#ff0000" width="2" height="2" depth="2"></a-box>
    <a-box position="-3 0.5 -20" color="#ff0000" width="2" height="2" depth="2"></a-box>

    <!-- 環境光源 -->
    <a-light type="ambient" color="#ffffff" intensity="0.5"></a-light>
    <a-light type="directional" color="#ffffff" intensity="1" position="2 4 -3"></a-light>
</a-scene>

</body>
</html>
