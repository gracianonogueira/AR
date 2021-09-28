<script src=”https://aframe.io/releases/0.6.1/aframe.min.js"></script>
<script src=”https://jeromeetienne.github.io/AR.js/aframe/build/aframe-ar.js"></script>

<body style=’margin : 0px; overflow: hidden;’>
  <a-scene embedded arjs=’sourceType: webcam;’>
      <a-marker preset=’hiro’>
        <!-- Adding an OBJ file to an AR Project-->
        <a-entity 
            obj-model=”obj: url(/path/to/nameOfFile.obj); 
            mtl: url(/path/to/nameOfFile.mtl)”>
        </a-entity>
              
      </a-marker>
  <a-entity camera>
  </a-entity>
  </a-scene>
</body>
