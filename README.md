Here is a simple HTML document that creates an index page listing links to sub-pages.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Subpage Index</title>
    <style>
        /* Simple, clean styling */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            background: #f9fafc;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 1.5rem;
        }

        .index-container {
            max-width: 900px;
            width: 100%;
            background: white;
            border-radius: 2rem;
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.06), 0 4px 8px rgba(0, 0, 0, 0.02);
            padding: 2.5rem 2rem;
            border: 1px solid rgba(255, 255, 255, 0.6);
            backdrop-filter: blur(2px);
        }

        h1 {
            font-size: 2.2rem;
            font-weight: 600;
            letter-spacing: -0.02em;
            color: #1a1e2c;
            display: flex;
            align-items: center;
            gap: 0.75rem;
            margin-bottom: 0.5rem;
            border-bottom: 2px solid #eef2f6;
            padding-bottom: 1.25rem;
        }

        h1 span {
            background: #eef2ff;
            color: #2d3b6e;
            font-size: 1.25rem;
            font-weight: 500;
            padding: 0.2rem 1rem;
            border-radius: 40px;
            letter-spacing: 0.3px;
        }

        .subtitle {
            color: #5b677b;
            font-size: 1rem;
            margin-bottom: 2.25rem;
            margin-top: 0.5rem;
            padding-left: 0.2rem;
        }

        .page-list {
            display: flex;
            flex-direction: column;
            gap: 0.6rem;
            list-style: none;
        }

        .page-list li {
            border-radius: 14px;
            transition: background 0.15s ease, transform 0.1s ease;
            border: 1px solid transparent;
        }

        .page-list li:hover {
            background: #f5f9ff;
            border-color: #dbe7fc;
            transform: translateX(6px);
        }

        .page-link {
            display: flex;
            align-items: center;
            padding: 1rem 1.5rem;
            text-decoration: none;
            color: #1f2a44;
            font-weight: 500;
            font-size: 1.15rem;
            border-radius: 14px;
            gap: 1rem;
            transition: color 0.15s;
        }

        .page-link:hover {
            color: #0a2540;
        }

        .page-icon {
            font-size: 1.5rem;
            line-height: 1;
            width: 2rem;
            text-align: center;
            opacity: 0.8;
        }

        .page-name {
            flex: 1;
        }

        .page-badge {
            background: #e6edf8;
            color: #2a3f6e;
            font-size: 0.75rem;
            font-weight: 600;
            padding: 0.2rem 0.75rem;
            border-radius: 30px;
            letter-spacing: 0.3px;
            text-transform: uppercase;
            border: 1px solid #cddcf0;
        }

        /* small extra style for empty state - not used but ready */
        .empty-message {
            color: #7a879b;
            padding: 1.5rem;
            text-align: center;
            font-style: italic;
        }

        footer {
            margin-top: 2rem;
            color: #98a6ba;
            font-size: 0.85rem;
            text-align: center;
            width: 100%;
        }

        /* For very small screens */
        @media (max-width: 500px) {
            .index-container {
                padding: 1.8rem 1.2rem;
            }

            h1 {
                font-size: 1.8rem;
                flex-wrap: wrap;
            }

            .page-link {
                padding: 0.9rem 1rem;
                font-size: 1rem;
                flex-wrap: wrap;
            }

            .page-badge {
                margin-left: auto;
            }
        }
    </style>
</head>
<body>
    <div class="index-container">
        <h1>
            📋 Page index
            <span>5 subpages</span>
        </h1>
        <p class="subtitle">Quick links to all sub pages in this directory</p>

        <ul class="page-list">
            <!-- 
                Replace the href values with your actual subpage filenames.
                These are examples using .html files.
            -->
            <li>
                <a href="about.html" class="page-link">
                    <span class="page-icon">📄</span>
                    <span class="page-name">About us</span>
                    <span class="page-badge">about.html</span>
                </a>
            </li>
            <li>
                <a href="services.html" class="page-link">
                    <span class="page-icon">🛠️</span>
                    <span class="page-name">Services</span>
                    <span class="page-badge">services.html</span>
                </a>
            </li>
            <li>
                <a href="products.html" class="page-link">
                    <span class="page-icon">📦</span>
                    <span class="page-name">Products</span>
                    <span class="page-badge">products.html</span>
                </a>
            </li>
            <li>
                <a href="portfolio.html" class="page-link">
                    <span class="page-icon">🎨</span>
                    <span class="page-name">Portfolio</span>
                    <span class="page-badge">portfolio.html</span>
                </a>
            </li>
            <li>
                <a href="contact.html" class="page-link">
                    <span class="page-icon">✉️</span>
                    <span class="page-name">Contact</span>
                    <span class="page-badge">contact.html</span>
                </a>
            </li>
        </ul>
    </div>

    <footer>Simple index page · click any link to navigate</footer>
</body>
</html>
```
