# dynamic-julia-set

<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dynamic Julia</title>
  <link rel="stylesheet" href="./css/style.css">
</head>
<body>
    <div class="sidebar">
        <div class="menu-item">
            <label for="param1">実部の初期値</label>
            <input type="number" id="param1" step="0.1" value="-0.4">
        </div>
        <div class="menu-item">
            <label for="param2">虚部の初期値</label>
            <input type="number" id="param2" step="0.1" value="0.6">
        </div>
        <div class="menu-item">
            <label for="param3">指数</label>
            <input type="number" id="param3" step="0.1" value="2">
        </div>
        <div class="menu-item">
            <label for="speed">アニメーション速度 (0.0001 - 0.01)</label>
            <input type="number" id="speed" step="0.0001" min="0.0001" max="0.01" value="0.0005">
        </div>
        <button onclick="startAnimation()">描画開始</button>
        <button onclick="stopAnimation()">描画停止</button>
    </div>
    <div class="main-content">
        <canvas id="fractalCanvas" width="600" height="600"></canvas>
    </div>


  <script src="script.js"></script>
</body>
</html>
