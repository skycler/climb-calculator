# Climbing Calculator

Create a fully self-contained, single-file web app (HTML, CSS, JavaScript) that calculates and visualizes the estimated average power output (in watts and watts per kilogram body weight) for climbing a mountain pass by road bike.

The app should:

🔢 Inputs:
- Body weight (kg)
- Material weight (bike + gear) (kg)
- two possibilities for climbing performance (tabs)
- Opton 1:
    - Total elevation gain (m)
    - Total distance (km)
    - Climb time (minutes and seconds)
- Option 2:
    - Hill slope (%)
    - Riding speed (km/h)

⚙️ Coefficients:
- Aerodynamic drag area (CdA)
- Rolling resistance coefficient (Crr)
- Mechanical efficiency (0–1)
- A dropdown with selectable coefficient presets:
    - Default (road bike): CdA = 0.35, Crr = 0.004, eta = 0.97
    - Aero setup (TT bike): CdA = 0.25, Crr = 0.003, eta = 0.98
    - MTB or gravel: CdA = 0.45, Crr = 0.008, eta = 0.96
    - Tour de France (climbing pro): CdA = 0.30, Crr = 0.004, eta = 0.98
    - Custom: allows editing all coefficients manually

📊 Output:
- Total average power in watts and W/kg (rounded and clearly displayed)
- A stacked horizontal bar chart showing the breakdown of power losses:
    - Gravity
    - Rolling resistance
    - Aerodynamic drag
    - Mechanical loss (due to η)

🎨 Style & Layout:
- Clean, modern, mobile-friendly UI
- Responsive grid layout for inputs
- Styled using lightweight custom CSS (no frameworks)
- Clear typography and spacing
- Shadowed cards, buttons, and bar chart styling

📈 Chart:
- Use Chart.js (import via CDN)
- Horizontal stacked bar chart for power component breakdown
- Tooltip showing exact watt values per segment

⚙️ Technical Notes:
- All code should be in one .html file
- No external assets besides Chart.js CDN
- JavaScript should recalculate immediately when pressing "Calculate"
- Pre-fill inputs with example values
- Run fully offline

Please generate and format the entire working code in one block.