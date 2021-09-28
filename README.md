
<html>
  <body>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/92/three.min.js"></script>
    <script>
      const scene = new THREE.Scene();
      const camera = new THREE.PerspectiveCamera(75, window.innerWidth/window.innerHeight, 1, 10000);
      const renderer = new THREE.WebGLRenderer();
      
      renderer.setSize(window.innerWidth, window.innerHeight);
      document.body.appendChild(renderer.domElement);
      
      const geometry = new THREE.BoxGeometry(500, 500, 500);
      const material = new THREE.MeshBasicMaterial({color: 0x00ff00, wireframe: true});
      const cube = new THREE.Mesh(geometry, material);
      
      scene.add(cube);
      camera.position.z = 1000;
      
      function render() {
        requestAnimationFrame(render);
        cube.rotation.x += 0.01;
        cube.rotation.y += 0.01;
        renderer.render(scene, camera);
      };
      
      render();
    </script>
  </body>
</html>
view raw
box_example.html hosted with ❤ by GitHub
