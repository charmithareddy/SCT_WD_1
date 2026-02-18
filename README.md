# SCT_WD_1
Responsive landing page
const navbar = document.getElementById("navbar");
const navLinks = navbar.querySelectorAll("a");

window.addEventListener("scroll", () => {
  if (window.scrollY > 60) {
    navbar.style.background = "#1e1e1e";
    navbar.style.boxShadow = "0 2px 8px rgba(0,0,0,0.3)";
  } else {
    navbar.style.background = "transparent";
    navbar.style.boxShadow = "none";
  }
});

navLinks.forEach(link => {
  link.addEventListener("mouseenter", () => {
    link.style.color = "#000";
    link.style.background = "#fff";
    link.style.borderRadius = "4px";
  });

  link.addEventListener("mouseleave", () => {
    link.style.color = "#fff";
    link.style.background = "transparent";
  });
});
