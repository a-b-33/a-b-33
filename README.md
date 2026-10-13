<!-- UNDERWATER AQUATIC THEME ANIMATION -->
<div style="
  width: 100%; 
  background: linear-gradient(180deg, #0f2027 0%, #203a43 50%, #2c5364 100%); 
  position: relative; 
  padding: 40px 20px; 
  border-radius: 12px; 
  overflow: hidden; 
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #e0f7fa;
  box-sizing: border-box;
">

  <!-- ANIMATING WATER RAYS & FLOW EFFECT -->
  <div style="
    position: absolute; 
    top: 0; left: 0; right: 0; bottom: 0; 
    background: radial-gradient(circle at 50% -20%, rgba(0, 229, 255, 0.15), transparent 60%); 
    pointer-events: none;
  "></div>

  <!-- FLOATING BUBBLES -->
  <div style="position: absolute; bottom: -20px; left: 10%; width: 8px; height: 8px; background: rgba(255,255,255,0.3); border-radius: 50%; animation: floatUp 8s infinite linear;"></div>
  <div style="position: absolute; bottom: -20px; left: 40%; width: 12px; height: 12px; background: rgba(255,255,255,0.2); border-radius: 50%; animation: floatUp 12s infinite linear; animation-delay: 2s;"></div>
  <div style="position: absolute; bottom: -20px; left: 75%; width: 6px; height: 6px; background: rgba(255,255,255,0.4); border-radius: 50%; animation: floatUp 6s infinite linear; animation-delay: 4s;"></div>

  <!-- SWIMMING FISH 1 (Left to Right) -->
  <div style="
    position: absolute; 
    top: 25%; 
    left: -50px; 
    font-size: 24px; 
    animation: swimRight 16s infinite linear;
    pointer-events: none;
  ">🐠</div>

  <!-- SWIMMING FISH 2 (Right to Left) -->
  <div style="
    position: absolute; 
    top: 55%; 
    right: -50px; 
    font-size: 20px; 
    animation: swimLeft 20s infinite linear;
    pointer-events: none;
  ">🐟</div>

  <!-- MAIN PROFILE CONTENT -->
  <div style="position: relative; z-index: 10; max-width: 600px; margin: 0 auto; text-align: center;">
    <h1 style="color: #00e5ff; margin-bottom: 10px; font-weight: 400; letter-spacing: 2px;">
      🐳 Welcome to My Deep Ocean
    </h1>
    <p style="color: #b2ebf2; font-size: 16px; margin-bottom: 30px; font-style: italic;">
      "Coding below the surface, exploring the digital currents."
    </p>

    <!-- SOCIAL / ACCOUNTS SECTION -->
    <div style="display: flex; justify-content: center; gap: 20px; margin-top: 20px;">
      <a href="https://leetcode.com" target="_blank" style="
        background: rgba(0, 229, 255, 0.1); 
        border: 1px solid rgba(0, 229, 255, 0.4); 
        padding: 10px 20px; 
        border-radius: 20px; 
        color: #00e5ff; 
        text-decoration: none; 
        font-weight: 600;
        transition: 0.3s;
      ">
        🚀 LeetCode: skd-33
      </a>
      <a href="https://dev.to" target="_blank" style="
        background: rgba(0, 229, 255, 0.1); 
        border: 1px solid rgba(0, 229, 255, 0.4); 
        padding: 10px 20px; 
        border-radius: 20px; 
        color: #00e5ff; 
        text-decoration: none; 
        font-weight: 600;
        transition: 0.3s;
      ">
        👩‍💻 Dev.to: ab_33
      </a>
    </div>
  </div>

  <!-- OCEAN FLOOR CORAL & GRASS SECTION -->
  <div style="
    position: absolute; 
    bottom: 0; 
    left: 0; 
    right: 0; 
    display: flex; 
    justify-content: space-around; 
    align-items: flex-end; 
    padding: 0 10px;
    pointer-events: none;
  ">
    <!-- Coral Grass Left -->
    <div style="font-size: 32px; transform-origin: bottom center; animation: sway 4s infinite ease-in-out;">🪸</div>
    <div style="font-size: 28px; transform-origin: bottom center; animation: sway 3.5s infinite ease-in-out; animation-delay: 0.5s; margin-left: -15px;">🌿</div>
    
    <!-- Center Empty for Text Readability -->
    <div></div>
    <div></div>

    <!-- Coral Grass Right -->
    <div style="font-size: 26px; transform-origin: bottom center; animation: sway 5s infinite ease-in-out; margin-right: -15px;">🌿</div>
    <div style="font-size: 35px; transform-origin: bottom center; animation: sway 4.5s infinite ease-in-out;">🪸</div>
  </div>

</div>

<!-- ANIMATION ENGINE (CSS KEYFRAMES) -->
<style>
  @keyframes swimRight {
    0% { transform: translateX(0px) scaleX(1); left: -50px; }
    100% { transform: translateX(calc(100% + 100vw)) scaleX(1); left: -50px; }
  }
  @keyframes swimLeft {
    0% { transform: translateX(0px) scaleX(1); right: -50px; }
    100% { transform: translateX(calc(-100% - 100vw)) scaleX(1); right: -50px; }
  }
  @keyframes sway {
    0%, 100% { transform: rotate(-5deg); }
    50% { transform: rotate(5deg); }
  }
  @keyframes floatUp {
    0% { transform: translateY(0) translateX(0); opacity: 0; }
    10% { opacity: 0.4; }
    90% { opacity: 0.4; }
    100% { transform: translateY(-300px) translateX(20px); opacity: 0; }
  }
</style>
