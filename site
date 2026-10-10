<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Advocacy Helpline Training</title>
<style>
  body { font-family: Arial, sans-serif; margin: 0; display: flex; height: 100vh; color: #333; }
  .sidebar { width: 250px; background: #f4f4f9; padding: 20px; border-right: 1px solid #ddd; }
  .sidebar h3 { margin-top: 0; font-size: 16px; border-bottom: 2px solid #0056b3; padding-bottom: 5px; }
  .nav-btn { display: block; width: 100%; text-align: left; background: none; border: none; padding: 10px 5px; cursor: pointer; color: #444; font-size: 14px; margin-bottom: 5px; }
  .nav-btn.active { font-weight: bold; color: #0056b3; }
  .nav-btn:disabled { color: #aaa; cursor: not-allowed; }
  .content { flex-grow: 1; padding: 40px; overflow-y: auto; }
  .module { display: none; max-width: 800px; }
  .module.active { display: block; }
  .quiz-section { background: #eef; padding: 15px; margin-top: 20px; border-radius: 5px; }
  button.unlock-btn { background: #0056b3; color: white; border: none; padding: 10px 15px; cursor: pointer; border-radius: 4px; margin-top: 10px; }
  button.unlock-btn:hover { background: #004494; }
</style>
</head>
<body>

<div class="sidebar">
  <h3>Course Modules</h3>
  <button class="nav-btn active" onclick="showModule('home')" id="nav-home">Start Here</button>
  <button class="nav-btn" onclick="showModule('mod1')" id="nav-mod1">Module 1: Know Your Role</button>
  <button class="nav-btn" onclick="showModule('mod2')" id="nav-mod2" disabled>Module 2: Distressed Callers 🔒</button>
  <button class="nav-btn" onclick="showModule('mod3')" id="nav-mod3" disabled>Module 3: Call Changes 🔒</button>
  <button class="nav-btn" onclick="showModule('mod4')" id="nav-mod4" disabled>Module 4: Correct Pathway 🔒</button>
  <button class="nav-btn" onclick="showModule('mod5')" id="nav-mod5" disabled>Module 5: Call Scenarios 🔒</button>
  <button class="nav-btn" onclick="showModule('final')" id="nav-final" disabled>Final Assessment 🔒</button>
</div>

<div class="content">
  <div id="home" class="module active">
    <h2>Start Here</h2>
    <p>Welcome to the Advocacy Helpline training. Purpose: practice consistent decisions when callers seek basic-needs, health, mental-health, reporting, and campus services.</p>
    <button class="unlock-btn" onclick="unlockNext('mod1')">Begin Module 1</button>
  </div>

  <div id="mod1" class="module">
    <h2>Module 1 | Know Your Role</h2>
    <p>Distinguish helpline resource/referral work from counseling, diagnosis, and crisis intervention.</p>
    <div class="quiz-section">
      <p><em>(Embed Google Form Quiz Link Here)</em></p>
      <button class="unlock-btn" onclick="unlockNext('mod2')">I scored 80% - Unlock Module 2</button>
    </div>
  </div>

  <div id="mod2" class="module">
    <h2>Module 2 | Communicating With a Distressed Caller</h2>
    <p>Supportive communication is calm, brief, nonjudgmental, and action-oriented.</p>
    <div class="quiz-section">
      <button class="unlock-btn" onclick="unlockNext('mod3')">I scored 80% - Unlock Module 3</button>
    </div>
  </div>

  <div id="mod3" class="module">
    <h2>Module 3 | Recognize When the Call Changes</h2>
    <p>Sometimes an ordinary referral call contains a new safety, mental-health, violence, or urgent basic-needs concern.</p>
    <div class="quiz-section">
      <button class="unlock-btn" onclick="unlockNext('mod4')">I scored 80% - Unlock Module 4</button>
    </div>
  </div>

  <div id="mod4" class="module">
    <h2>Module 4 | Choose the Correct Pathway</h2>
    <p>The correct next step depends on the caller’s need, eligibility, home college, existing activity, and urgency.</p>
    <div class="quiz-section">
      <button class="unlock-btn" onclick="unlockNext('mod5')">I scored 80% - Unlock Module 5</button>
    </div>
  </div>

  <div id="mod5" class="module">
    <h2>Module 5 | Apply It: Call Scenarios</h2>
    <p>Use the same four-question framework consistently even when needs overlap.</p>
    <div class="quiz-section">
      <button class="unlock-btn" onclick="unlockNext('final')">I scored 80% - Unlock Final Assessment</button>
    </div>
  </div>

  <div id="final" class="module">
    <h2>Comprehensive Final Assessment</h2>
    <p>Complete the 10 scored items to finish your certification.</p>
    <p><em>(Embed Final Google Form Here)</em></p>
  </div>
</div>

<script>
  function showModule(modId) {
    document.querySelectorAll('.module').forEach(m => m.classList.remove('active'));
    document.querySelectorAll('.nav-btn').forEach(b => b.classList.remove('active'));
    
    document.getElementById(modId).classList.add('active');
    document.getElementById('nav-' + modId).classList.add('active');
  }

  function unlockNext(nextModId) {
    let nextBtn = document.getElementById('nav-' + nextModId);
    nextBtn.disabled = false;
    nextBtn.innerText = nextBtn.innerText.replace(' 🔒', '');
    showModule(nextModId);
  }
</script>

</body>
</html>
