# MastitisGuard AI · 3D Animal Wearable Digital Twin
### Team SPIRIT (H14_SPIRIT) · Interactive Hardware DFM & Exploded Assembly Model

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com)

An interactive, photorealistic 3D engineering digital twin of the **MastitisGuard AI Animal Wearable** built from the official engineering schematics and reference CAD designs. Designed for seamless presentation, hardware inspection, and 1-click deployment on **Render**.

---

## 🌟 Highlights & Features

- **Reference-Accurate CAD Architecture**: Reconstructed from the official exploded assembly schematic:
  - **01 Top Cover**: Ruggedized IP65 ABS/Polycarbonate lid with corner counterbores, side shock flanges, and recessed label/barcode plate.
  - **02 Sealing Gasket**: IP67 continuous fluorosilicone/EPDM elastomeric seal.
  - **03 Antenna Module (GPS NEO-6M)**: High-dielectric ceramic patch antenna with center silver electrode and golden RF ground plane.
  - **04 Main Compute PCB (77.0 × 61.0 mm)**: SMT assembly with ESP32-WROOM laser-etched metal RF shield can, golden serpentine inverted-F PCB antenna, dual 15-pin headers, MPU6050 6-axis motion sensor, MAX30205 clinical temperature sensor, axial resistors (R1, R2), and official `H14_SPIRIT` / `Spirit` silkscreen artwork.
  - **05 Li-ion Battery Pack (18650)**: Cylindrical cell (18.4 × 65.2 mm, 3.7V 2600mAh, 9.62Wh) with authentic foil label, crimp groove, and red/black silicone lead wires.
  - **06 Bottom Enclosure**: Deep IP65 tub with internal battery retention ribs, 3 front-side circular port cutouts, and integrated collar strap lugs with hinge pins.
  - **Fasteners**: 4× top M3 Allen socket screws + 4× bottom screws with flat washers.
  - **Collar Strap Assembly**: Matte industrial collar with 3 rectangular ventilation/sizing slots matching the top-view assembled diagram.
- **Interactive Exploded View**: Smooth slider from 0% (mated/assembled) to 100% (exploded) with automated quick-explode animation and blue datum trace guide lines.
- **3D Floating Badges (01 to 06)**: Interactive pins floating in 3D space matching the numbered reference annotations.
- **Click-to-Inspect Drawer**: Click any component or 3D pin to zoom in, trigger an emissive pulse, and view material grade, IP rating, dimensions, fasteners, and manufacturing notes.
- **X-Ray / Cutaway Housing**: Toggle translucent enclosure mode to reveal internal PCB, battery, and sensors while fully assembled.
- **Camera Presets**: One-click camera switches for **Exploded Iso**, **Top Assembled**, **PCB Top Silk Macro**, and **Side Profile**.
- **High-Res 4K Export**: One-click PNG snapshot capture with clean studio lighting.
- **Turntable Mode**: Smooth 360° continuous turntable rotation for presentations.

---

## 🚀 How to Deploy on Render (Zero-Configuration)

### Option A: Render Static Site (Recommended · 100% Free & Instant)

1. **Push this folder to GitHub / GitLab**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit of MastitisGuard 3D Twin"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/mastitisguard-3d.git
   git push -u origin main
   ```

2. **Log into [Render.com](https://dashboard.render.com/)**:
   - Click **New +** and select **Static Site**.
   - Connect your GitHub repository.
   - Configure the following settings (most are auto-detected):
     - **Name**: `mastitisguard-3d` (or your preferred name)
     - **Branch**: `main`
     - **Build Command**: *(leave empty)*
     - **Publish Directory**: `.`
   - Click **Create Static Site**.
   - Your 3D digital twin will be live with free global CDN and HTTPS in under 60 seconds!

---

### Option B: Deploy via Render Blueprint (`render.yaml`)

This repository includes a pre-configured `render.yaml` file:

1. Push the code to your Git provider.
2. In Render Dashboard, click **New +** > **Blueprint**.
3. Select your repository.
4. Render will automatically read `render.yaml` and provision the static site with zero manual input!

---

### Option C: Render Web Service (Node.js)

If your team prefers deploying as a Node.js Web Service:
- **Build Command**: *(leave empty)*
- **Start Command**: `node server.js`
- Render will start the built-in HTTP server on `process.env.PORT`.

---

## 💻 Running Locally

You don't need any complex build tools (Webpack, Vite, or Babel). Everything runs natively in any modern browser.

### Method 1: Using Node.js
```bash
node server.js
```
Open [http://localhost:3000](http://localhost:3000) in your web browser.

### Method 2: Using Python
```bash
# Python 3
python -m http.server 3000
```
Open [http://localhost:3000](http://localhost:3000) in your web browser.

### Method 3: Direct File Opening
Double-click `index.html` to open it directly in Google Chrome, Microsoft Edge, Firefox, or Safari with WebGL enabled.

---

## 📐 Hardware Architecture Summary (H14_SPIRIT)

| Component | BOM Ref | Material / Model | Key Specification |
|---|---|---|---|
| **Top Cover** | `MG-01-TC` | ABS/Polycarbonate | 86.0 × 72.0 × 16.0 mm, IP65 sealed |
| **Sealing Gasket** | `MG-02-SG` | Fluorosilicone / EPDM | 82.5 × 68.5 × 2.8 mm, Shore A 55, IP67 |
| **Antenna Module** | `MG-03-GPS` | Ceramic Dielectric | 25.0 × 25.0 × 4.2 mm, NEO-6M L1 GPS patch |
| **Compute PCB** | `MG-04-PCB` | 4-Layer FR4 ENIG | 77.0 × 61.0 × 1.6 mm, ESP32 + MPU6050 + MAX30205 |
| **Battery Cell** | `MG-05-BAT` | Li-ion 18650 | 3.7V 2600mAh (9.62Wh), 6–12 mo. autonomy |
| **Bottom Enclosure** | `MG-06-BE` | ABS/Polycarbonate | 86.0 × 72.0 × 20.0 mm, 3 side ports, strap mounts |
| **Collar Strap** | `MG-07-ST` | Fluoroelastomer | 3 rectangular vent slots, stainless hinge pins |
| **Fasteners** | `MG-08-SC` | A2 Stainless Steel | 4× M3×10mm Top Allen + 4× M3 Bottom Screws |

---

## 🛡️ License & Attribution

- **Project**: MastitisGuard AI (SIH PS SH26109)
- **Team**: Team SPIRIT (`H14_SPIRIT`)
- **License**: MIT License
