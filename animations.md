<link rel="stylesheet" href="style.css">

# My Animation Page

<div class="fade-in">
  Hello! This text fades in.
</div>


# Scroll Animation Example

<div style="height: 500px;">
  Scroll down to see the animation.
</div>

<div class="scroll-fade">
  This text fades in when you scroll to it.
</div>

<div style="height: 500px;"></div>

<div class="scroll-fade">
  This one also replays when you scroll back to it.
</div>



<script>
const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.remove("animate");

      // Forces the animation to restart
      void entry.target.offsetWidth;

      entry.target.classList.add("animate");
    } else {
      entry.target.classList.remove("animate");
    }
  });
});

document.querySelectorAll(".scroll-fade").forEach(element => {
  observer.observe(element);
});
</script>


text
text
text
text
text
text
text
text
text
text
text
text




text






text







text







texttext






text






text
