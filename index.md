---
layout: page
title: "Home"
---

<!-- Hero Section -->
<div class="hero">
    <h1 id="greeting"></h1>
</div>

<h2>Welcome!</h2>
<p>Experience a beautifully designed website with interactive features.</p>

<script>
    const now = new Date();
    const hours = now.getHours();
    let greeting;

    if (hours < 12) {
        greeting = "Good Morning!";
    } else if (hours < 18) {
        greeting = "Good Afternoon!";
    } else {
        greeting = "Good Evening!";
    }

    document.getElementById('greeting').textContent = greeting;
</script>
