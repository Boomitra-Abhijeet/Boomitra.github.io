# 🌱 Boomitra Carbon Credit Buy Widget

A lightweight, self-contained widget that allows users to purchase and offset carbon credits directly from any webpage using Boomitra’s verified agricultural regeneration projects.

## ⚙️ Integration

Simply include the hosted SDK script and add a widget container <div>.

Inline Mode (embed directly in page):
<script src="https://cdn-boomitra-dev.s3.ap-south-1.amazonaws.com/sales-widget/carbon-widget.js"></script>
<div data-mode="inline" data-sandbox="true"></div>

Floating Mode (popup button):
<script src="https://cdn-boomitra-dev.s3.ap-south-1.amazonaws.com/sales-widget/carbon-widget.js"></script>
<div data-mode="floating" data-sandbox="true"></div>

## 🧪 Sandbox vs Production

Use the data-sandbox attribute to switch between environments:
- data-sandbox="true" → Sandbox (test mode, no real payments)
- data-sandbox="false" or omitted → Production (live payments)

## 💡 How It Works

1. User enters number of carbon credits to offset.
2. Provides contact info and confirms payment.
3. Secure Helcim payment popup opens.
4. On success, user is redirected to Boomitra’s success page.

## ✅ Summary

| Feature | Inline | Floating |
|----------|---------|-----------|
| Appears inside page | ✅ | ❌ |
| Opens as popup | ❌ | ✅ |
| Sandbox support | ✅ | ✅ |
| Self-contained | ✅ | ✅ |

Example (Floating Mode Sandbox):
<!doctype html>
<html>
<head>
  <meta charset="utf-8" />
  <title>Carbon Credit Buy Widget</title>
  <script src="https://cdn-boomitra-dev.s3.ap-south-1.amazonaws.com/sales-widget/carbon-widget.js"></script>
</head>
<body>
  <div data-mode="floating" data-sandbox="true"></div>
</body>
</html>

🧰 Developer Tip: Run CarbonWidgetDebug() in your browser console to reload widget styles without reloading the page.
