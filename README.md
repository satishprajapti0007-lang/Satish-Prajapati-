# Satish-Prajapati-
Fune 
function yesClicked() {
    window.location.href = "yes.html";
}

const noBtn = document.getElementById("noBtn");

function moveNo() {
    let x = Math.random() * 300 - 150;
    let y = Math.random() * 300 - 150;

    noBtn.style.transform = `translate(${x}px, ${y}px)`;
}

// PC
noBtn.addEventListener("mouseover", moveNo);

// Mobile
noBtn.addEventListener("touchstart", function (e) {
    e.preventDefault(); // Stops the normal tap
    moveNo();
});

// Extra support
noBtn.addEventListener("click", function (e) {
    e.preventDefault();
    moveNo();
});
