<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Two-Slit Interference</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
      background: #f7f7f7;
      color: #222;
    }
    .panel {
      background: white;
      border-radius: 12px;
      padding: 16px;
      margin-bottom: 16px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.08);
    }
    .row {
      display: flex;
      gap: 16px;
      flex-wrap: wrap;
      align-items: center;
      margin-bottom: 8px;
    }
    canvas {
      border: 1px solid #ccc;
      border-radius: 8px;
      background: black;
      display: block;
      margin-top: 12px;
      max-width: 100%;
    }
    input[type="range"] {
      width: 220px;
    }
    button {
      padding: 8px 12px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div class="panel">
    <h1>Young's Two-Slit Interference</h1>
    <p>The displayed field is the sum of two coherent point-source waves.</p>

    <div class="row">
      <label>Slit separation d
        <input id="dSlider" type="range" min="20" max="220" step="1" value="80">
      </label>
      <span id="dVal">80</span>

      <label>Wavelength lambda
        <input id="lambdaSlider" type="range" min="10" max="120" step="1" value="40">
      </label>
      <span id="lambdaVal">40</span>

      <label>Amplitude A
        <input id="ampSlider" type="range" min="0.2" max="5" step="0.1" value="2">
      </label>
      <span id="ampVal">2.0</span>
    </div>

    <div class="row">
      <button id="toggleBtn">Pause</button>
    </div>

    <canvas id="canvas" width="900" height="500"></canvas>
  </div>

  <script>
    const canvas = document.getElementById("canvas");
    const ctx = canvas.getContext("2d");

    const dSlider = document.getElementById("dSlider");
    const lambdaSlider = document.getElementById("lambdaSlider");
    const ampSlider = document.getElementById("ampSlider");

    const dVal = document.getElementById("dVal");
    const lambdaVal = document.getElementById("lambdaVal");
    const ampVal = document.getElementById("ampVal");

    const toggleBtn = document.getElementById("toggleBtn");

    let time = 0;
    let running = true;

    function updateLabels() {
      dVal.textContent = dSlider.value;
      lambdaVal.textContent = lambdaSlider.value;
      ampVal.textContent = ampSlider.value;
    }

    [dSlider, lambdaSlider, ampSlider].forEach(el => {
      el.addEventListener("input", updateLabels);
    });

    toggleBtn.addEventListener("click", () => {
      running = !running;
      toggleBtn.textContent = running ? "Pause" : "Resume";
    });

    function render() {
      const width = canvas.width;
      const height = canvas.height;
      const img = ctx.createImageData(width, height);
      const data = img.data;

      const d = parseFloat(dSlider.value);
      const lambda = parseFloat(lambdaSlider.value);
      const A = parseFloat(ampSlider.value);
      const k = 2 * Math.PI / lambda;
      const omega = 4;

      const slitX = 120;
      const slitY1 = height / 2 - d / 2;
      const slitY2 = height / 2 + d / 2;

      const step = 3;

      for (let y = 0; y < height; y += step) {
        for (let x = 0; x < width; x += step) {
          const r1 = Math.sqrt((x - slitX) ** 2 + (y - slitY1) ** 2) + 1e-6;
          const r2 = Math.sqrt((x - slitX) ** 2 + (y - slitY2) ** 2) + 1e-6;

          const u =
            A / r1 * Math.sin(k * r1 - omega * time) +
            A / r2 * Math.sin(k * r2 - omega * time);

          const intensity = Math.max(0, Math.min(255, 128 + 127 * Math.tanh(6 * u)));

          for (let yy = 0; yy < step; yy++) {
            for (let xx = 0; xx < step; xx++) {
              const px = x + xx;
              const py = y + yy;
              if (px < width && py < height) {
                const idx = (py * width + px) * 4;
                data[idx] = intensity;
                data[idx + 1] = intensity;
                data[idx + 2] = 255;
                data[idx + 3] = 255;
              }
            }
          }
        }
      }

      ctx.putImageData(img, 0, 0);

      ctx.fillStyle = "white";
      ctx.fillRect(slitX - 4, 0, 8, height);

      ctx.fillStyle = "black";
      ctx.fillRect(slitX - 6, slitY1 - 6, 12, 12);
      ctx.fillRect(slitX - 6, slitY2 - 6, 12, 12);

      ctx.fillStyle = "red";
      ctx.beginPath();
      ctx.arc(slitX, slitY1, 4, 0, 2 * Math.PI);
      ctx.fill();

      ctx.beginPath();
      ctx.arc(slitX, slitY2, 4, 0, 2 * Math.PI);
      ctx.fill();
    }

    function animate() {
      if (running) time += 0.05;
      render();
      requestAnimationFrame(animate);
    }

    updateLabels();
    animate();
  </script>
</body>
</html>