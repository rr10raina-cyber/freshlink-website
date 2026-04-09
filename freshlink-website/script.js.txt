function submitForm(e) {
    e.preventDefault();
    document.getElementById("msg").innerText =
    "✅ Thank you! Our team will contact you soon.";
}

window.addEventListener("scroll", () => {
    let reveals = document.querySelectorAll(".reveal");

    reveals.forEach((el) => {
        let windowHeight = window.innerHeight;
        let elementTop = el.getBoundingClientRect().top;

        if (elementTop < windowHeight - 100) {
            el.classList.add("active");
        }
    });
});