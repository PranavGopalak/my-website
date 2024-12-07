---
layout: page
title: "Random Quote"
---

<div class="quote-container">
    <blockquote id="quote">Loading quote...</blockquote>
    <cite id="author"></cite>
    <button onclick="generateQuote()">New Quote</button>
</div>

<script>
const quotes = [
    {
        text: "Believe you can and you're halfway there.",
        author: "Theodore Roosevelt"
    },
    {
        text: "Your time is limited, so don't waste it living someone else's life.",
        author: "Steve Jobs"
    },
    {
        text: "The only way to do great work is to love what you do.",
        author: "Steve Jobs"
    },
    {
        text: "If you can dream it, you can achieve it.",
        author: "Zig Ziglar"
    },
    {
        text: "The future belongs to those who believe in the beauty of their dreams.",
        author: "Eleanor Roosevelt"
    }
];

function generateQuote() {
    const randomIndex = Math.floor(Math.random() * quotes.length);
    const quote = quotes[randomIndex];

    document.getElementById('quote').textContent = quote.text;
    document.getElementById('author').textContent = `— ${quote.author}`;
}

// Generate a quote when the page loads
window.onload = generateQuote;
</script>
