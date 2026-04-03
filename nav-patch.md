# Nav patch for index.html
# Add this somewhere in your existing nav / bottom strip, styled to match.
# The splash page doesn't have a formal <nav> tag, so two options below:

## Option A — Add a subtle text link to the bottom strip
# Find your existing .bottom-strip div and add a third item:

  <div class="bottom-item">
    <a href="rental-data.html" style="color:rgba(255,255,255,0.55);text-decoration:none;letter-spacing:.05em;font-size:12px;">
      Rental Data →
    </a>
  </div>


## Option B — Add a minimal nav bar above the splash (insert before <div class="bg-layer">)

<nav style="
  position:fixed; top:0; left:0; right:0; z-index:100;
  display:flex; justify-content:flex-end; align-items:center;
  padding:0 32px; height:44px;
  background:rgba(18,36,72,0.7); backdrop-filter:blur(8px);
  border-bottom:0.5px solid rgba(255,255,255,0.1);
">
  <a href="rental-data.html" style="
    font-family:'DM Sans',sans-serif; font-size:12px; font-weight:500;
    letter-spacing:.06em; text-transform:uppercase;
    color:rgba(255,255,255,0.55); text-decoration:none;
    transition:color .15s;
  "
  onmouseover="this.style.color='rgba(255,255,255,0.9)'"
  onmouseout="this.style.color='rgba(255,255,255,0.55)'"
  >Rental Data →</a>
</nav>
