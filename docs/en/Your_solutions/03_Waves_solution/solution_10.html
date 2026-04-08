<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Wave Sources Superposition</title>
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
    canvas {
      border: 1px solid #ccc;
      border-radius: 8px;
      background: black;
      display: block;
      margin-top: 12px;
      max-width: 100%;
    }
    .row {
      display: flex;
      gap: 16px;
      flex-wrap: wrap;
      align-items: center;
      margin-bottom: 8px;
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
    <h1>Wave Sources Superposition</h1>
    <p>Click on the canvas to add sources. The field is</p>
    <p><code>u(r,t) = A / |r-r0|^alpha * sin(k |r-r0| - omega t)</code></p>

    <div class="row">
      <label>A <input id="amp" type="range" min="0.1" max="5" step="0.1" value="1.5"></label>
      <span id="ampVal">1.5</span>

      <label>alpha <input id="alpha" type="range" min="0" max="2" step="0.01" value="1"></label>
      <span id="alphaVal">1.00</span>

      <label>lambda <input id="lambda" type="range" min="10" max="120" step="1" value="40"></label>
      <span id="lambdaVal">40</span>

      <label>omega <input id="omega" type="range" min="0.5" max="12" step="0.1" value="4"></label>
      <span id="omegaVal">4.0</span>
    </div>

    <div class="row">
      <button id="clearBtn">Clear Sources</button>
      <button id="toggleBtn">Pause</button>
    </div>

    <canvas id="canvas" width="800" height="500"></canvas>
  </div>

  <script>
    const canvas = document.getElementById("canvas");
    const ctx = canvas.getContext("2d");

    const ampSlider = document.getElementById("amp");
    const alphaSlider = document.getElementById("alpha");
    const lambdaSlider = document.getElementById("lambda");
    const omegaSlider = document.getElementById("omega");

    const ampVal = document.getElementById("ampVal");
    const alphaVal = document.getElementById("alphaVal");
    const lambdaVal = document.getElementById("lambdaVal");
    const omegaVal = document.getElementById("omegaVal");

    const clearBtn = document.getElementById("clearBtn");
    const toggleBtn = document.getElementById("toggleBtn");

    const sources = [];
    let running = true;
    let time = 0;

    function updateLabels() {
      ampVal.textContent = ampSlider.value;
      alphaVal.textContent = Number(alphaSlider.value).toFixed(2);
      lambdaVal.textContent = lambdaSlider.value;
      omegaVal.textContent = omegaSlider.value;
    }

    canvas.addEventListener("click", (e) => {
      const rect = canvas.getBoundingClientRect();
      const x = (e.clientX - rect.left) * (canvas.width / rect.width);
      const y = (e.clientY - rect.top) * (canvas.height / rect.height);
      sources.push({ x, y });
    });

    clearBtn.addEventListener("click", () => {
      sources.length = 0;
    });

    toggleBtn.addEventListener("click", () => {
      running = !running;
      toggleBtn.textContent = running ? "Pause" : "Resume";
    });

    [ampSlider, alphaSlider, lambdaSlider, omegaSlider].forEach(el => {
      el.addEventListener("input", updateLabels);
    });

    function render() {
      const img = ctx.createImageData(canvas.width, canvas.height);
      const data = img.data;

      const A = parseFloat(ampSlider.value);
      const alpha = parseFloat(alphaSlider.value);
      const lambda = parseFloat(lambdaSlider.value);
      const omega = parseFloat(omegaSlider.value);
      const k = 2 * Math.PI / lambda;

      const step = 3;

      for (let y = 0; y < canvas.height; y += step) {
        for (let x = 0; x < canvas.width; x += step) {
          let u = 0;

          for (const s of sources) {
            const dx = x - s.x;
            const dy = y - s.y;
            const r = Math.sqrt(dx * dx + dy * dy) + 1e-6;
            u += A / Math.pow(r, alpha) * Math.sin(k * r - omega * time);
          }

          const intensity = Math.max(0, Math.min(255, 128 + 127 * Math.tanh(4 * u)));

          for (let yy = 0; yy < step; yy++) {
            for (let xx = 0; xx < step; xx++) {
              const px = x + xx;
              const py = y + yy;
              if (px < canvas.width && py < canvas.height) {
                const idx = (py * canvas.width + px) * 4;
                data[idx] = intensity;
                data[idx + 1] = 100;
                data[idx + 2] = 255 - intensity;
                data[idx + 3] = 255;
              }
            }
          }
        }
      }

      ctx.putImageData(img, 0, 0);

      for (const s of sources) {
        ctx.beginPath();
        ctx.arc(s.x, s.y, 5, 0, 2 * Math.PI);
        ctx.fillStyle = "white";
        ctx.fill();
      }
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