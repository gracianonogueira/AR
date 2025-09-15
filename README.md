<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Esfera em Realidade Aumentada</title>
    <script src="https://aframe.io/releases/1.3.0/aframe.min.js"></script>
    <script src="https://raw.githack.com/AR-js-org/AR.js/master/aframe/build/aframe-ar.js"></script>
    <style>
        body { margin: 0; overflow: hidden; }
        .ar-container {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }
    </style>
</head>
<body>
    <div class="ar-container">
        <a-scene embedded arjs>
            <a-marker preset="hiro">
                <a-sphere
                    position="0 0.5 0"
                    radius="0.5"
                    color="#FF0000"
                    shader="standard"
                    roughness="0.7"
                    metalness="0.5">
                </a-sphere>
            </a-marker>
            <a-entity camera></a-entity>
        </a-scene>
    </div>
</body>
</html>
