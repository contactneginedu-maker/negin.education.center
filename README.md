<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="مرکز آموزشی و توان‌بخشی نگین - مؤسسه خدماتی و حرفه‌ای زنان بی‌بضاعت. آموزش، توان‌بخشی و حمایت از کودکان دارای معلولیت و نیازهای آموزشی ویژه. هر کودک، یک نگین 💎">
    <title>مرکز آموزشی و توان‌بخشی نگین | مؤسسه خدماتی و حرفه‌ای زنان بی‌بضاعت</title>
    <style>
        /* =========================================================
           ROOT VARIABLES & THEME
        ========================================================= */
        :root {
            /* Primary Colors */
            --primary: #075985;
            --primary-dark: #043b4d;
            --primary-light: #0ea5e9;
            --primary-bg: #031e29;
            
            /* Accent Colors */
            --gold: #ffc800;
            --gold-dark: #c99d00;
            --gold-light: #ffe066;
            --accent: #e63946;
            
            /* Semantic Colors */
            --success: #28a745;
            --warning: #ffc107;
            --danger: #dc2626;
            --info: #17a2b8;
            
            /* Neutral Colors */
            --background: #f7fafc;
            --surface: #ffffff;
            --surface-soft: #eef5f8;
            --surface-hover: #e2edf2;
            --text: #172033;
            --text-soft: #475569;
            --text-light: #64748b;
            --text-muted: #94a3b8;
            --border: #d8e1e8;
            --border-strong: #cbd5e1;
            
            /* Shadows */
            --shadow-sm: 0 1px 3px rgba(0, 0, 0, 0.1);
            --shadow: 0 10px 35px rgba(15, 23, 42, 0.10);
            --shadow-lg: 0 20px 60px rgba(15, 23, 42, 0.15);
            
            /* Typography */
            --font-size-xs: 12px;
            --font-size-sm: 14px;
            --font-size-base: 16px;
            --font-size-lg: 18px;
            --font-size-xl: 20px;
            --font-size-2xl: 24px;
            --font-size-3xl: 30px;
            
            /* Spacing */
            --spacing-xs: 8px;
            --spacing-sm: 12px;
            --spacing-md: 16px;
            --spacing-lg: 24px;
            --spacing-xl: 32px;
            --spacing-2xl: 48px;
            
            /* Layout */
            --sidebar-width: 280px;
            --header-height: 140px;
            --nav-height: 60px;
            
            /* Transitions */
            --transition-fast: 0.2s ease;
            --transition: 0.3s ease;
            --transition-slow: 0.5s ease;
            
            /* Border Radius */
            --radius-sm: 8px;
            --radius: 12px;
            --radius-lg: 16px;
            --radius-xl: 20px;
            --radius-2xl: 28px;
            --radius-full: 50%;
        }

        /* =========================================================
           DARK MODE
        ========================================================= */
        body.dark {
            --background: #081419;
            --surface: #102129;
            --surface-soft: #142b34;
            --surface-hover: #1a3340;
            --text: #f1f5f9;
            --text-soft: #cbd5e1;
            --text-light: #a7b6c0;
            --text-muted: #788694;
            --border: #29404a;
            --border-strong: #3a505a;
            --shadow: 0 10px 35px rgba(0, 0, 0, 0.35);
            --shadow-lg: 0 20px 60px rgba(0, 0, 0, 0.45);
        }

        /* =========================================================
           HIGH CONTRAST MODE
        ========================================================= */
        body.high-contrast {
            --primary: #000000;
            --primary-dark: #000000;
            --primary-light: #111111;
            --gold: #ffff00;
            --gold-dark: #cccc00;
            --accent: #ff0000;
            --background: #ffffff;
            --surface: #ffffff;
            --surface-soft: #ffffff;
            --text: #000000;
            --text-soft: #000000;
            --text-light: #000000;
            --text-muted: #444444;
            --border: #000000;
            --border-strong: #000000;
            --shadow: 0 0 0 rgba(0, 0, 0, 0);
        }

        body.high-contrast.dark {
            --background: #000000;
            --surface: #000000;
            --surface-soft: #000000;
            --text: #ffffff;
            --text-soft: #ffffff;
            --text-light: #cccccc;
            --border: #ffffff;
            --gold: #ffff00;
        }

        /* =========================================================
           RESET & BASE STYLES
        ========================================================= */
        *, *::before, *::after {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html {
            font-size: 100%;
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Vazirmatn', 'Noto Sans Arabic', 'Tahoma', 'Arial', sans-serif;
            background: var(--background);
            color: var(--text);
            line-height: 1.8;
            direction: rtl;
            text-align: right;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            transition: var(--transition);
        }

        /* Focus Styles for Accessibility */
        :focus-visible {
            outline: 4px solid var(--gold);
            outline-offset: 3px;
        }

        button, input, select, textarea, a {
            font-family: inherit;
        }

        button {
            cursor: pointer;
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        a {
            color: var(--primary);
            text-decoration: none;
            transition: var(--transition-fast);
        }

        a:hover, a:focus {
            color: var(--primary-dark);
        }

        /* =========================================================
           TOP HEADER - مؤسسه نگین
        ========================================================= */
        .top-header {
            background: linear-gradient(135deg, var(--primary-dark) 0%, var(--primary) 100%);
            color: white;
            padding: var(--spacing-sm) var(--spacing-md);
            position: relative;
            overflow: hidden;
            z-index: 1000;
        }

        .top-header-container {
            max-width: 1400px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: relative;
            z-index: 2;
        }

        .header-logo-img {
            width: 60px;
            height: 60px;
            border-radius: var(--radius-full);
            object-fit: cover;
            flex-shrink: 0;
            margin-left: var(--spacing-sm);
        }

        .header-logo-text {
            line-height: 1.3;
        }

        .header-logo-text .institute {
            font-size: var(--font-size-sm);
            font-weight: 600;
            opacity: 0.9;
        }

        .header-logo-text .center {
            font-size: var(--font-size-xl);
            font-weight: 800;
            margin: 2px 0;
        }

        .header-logo-text .slogan {
            font-size: var(--font-size-sm);
            font-weight: 600;
            color: var(--gold);
            display: flex;
            align-items: center;
            gap: 5px;
        }

        .header-logo-text .slogan .gem {
            font-size: 1.2rem;
        }

        .header-nav {
            display: flex;
            gap: var(--spacing-sm);
            flex-wrap: wrap;
        }

        .header-nav a {
            color: white;
            padding: var(--spacing-xs) var(--spacing-sm);
            border-radius: var(--radius);
            font-size: var(--font-size-sm);
            font-weight: 600;
            transition: var(--transition-fast);
        }

        .header-nav a:hover,
        .header-nav a:focus {
            background: rgba(255, 255, 255, 0.15);
        }

        /* =========================================================
           IMAGE SLIDER (Background behind header)
        ========================================================= */
        .slider-container {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: var(--header-height);
            overflow: hidden;
            z-index: 1;
        }

        .slider {
            display: flex;
            height: 100%;
            transition: transform 1s ease-in-out;
        }

        .slide {
            min-width: 100%;
            height: 100%;
            position: relative;
        }

        .slide img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            opacity: 0.3;
        }

        .slide-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, rgba(7, 89, 133, 0.8), rgba(4, 59, 77, 0.9));
        }

        .slider-dots {
            position: absolute;
            bottom: var(--spacing-sm);
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            gap: var(--spacing-xs);
            z-index: 10;
        }

        .dot {
            width: 10px;
            height: 10px;
            border-radius: var(--radius-full);
            background: rgba(255, 255, 255, 0.5);
            cursor: pointer;
            transition: var(--transition-fast);
        }

        .dot.active {
            background: var(--gold);
            width: 25px;
            border-radius: 5px;
        }

        /* =========================================================
           ACCESSIBILITY BAR
        ========================================================= */
        .accessibility-bar {
            background: var(--primary-dark);
            color: white;
            padding: var(--spacing-xs) var(--spacing-md);
            display: flex;
            justify-content: flex-start;
            align-items: center;
            gap: var(--spacing-xs);
            flex-wrap: wrap;
            font-size: var(--font-size-sm);
        }

        .accessibility-bar strong {
            margin-right: var(--spacing-sm);
        }

        .accessibility-bar button {
            border: 1px solid rgba(255, 255, 255, 0.3);
            background: rgba(255, 255, 255, 0.1);
            color: white;
            padding: var(--spacing-xs) var(--spacing-sm);
            border-radius: var(--radius);
            font-size: var(--font-size-sm);
            transition: var(--transition-fast);
        }

        .accessibility-bar button:hover {
            background: var(--gold);
            color: #111;
            border-color: var(--gold);
        }

        /* =========================================================
           MAIN NAVIGATION
        ========================================================= */
        .main-nav {
            background: var(--surface);
            border-bottom: 1px solid var(--border);
            position: sticky;
            top: var(--header-height);
            z-index: 999;
            box-shadow: var(--shadow-sm);
        }

        .nav-container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 var(--spacing-md);
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: var(--nav-height);
        }

        .nav-logo {
            display: flex;
            align-items: center;
            gap: var(--spacing-sm);
            text-decoration: none;
            color: var(--text);
        }

        .nav-logo-icon {
            display: none;
        }

        .nav-logo-img {
            width: 40px;
            height: 40px;
            border-radius: var(--radius-full);
            object-fit: cover;
            flex-shrink: 0;
        }

        .nav-logo-text {
            font-weight: 700;
            font-size: var(--font-size-lg);
        }

        .nav-links {
            display: flex;
            gap: var(--spacing-sm);
            flex-wrap: wrap;
        }

        .nav-links a {
            padding: var(--spacing-xs) var(--spacing-sm);
            border-radius: var(--radius);
            font-weight: 600;
            font-size: var(--font-size-sm);
            transition: var(--transition-fast);
        }

        .nav-links a:hover,
        .nav-links a:focus {
            background: var(--surface-soft);
            color: var(--primary);
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--text);
            padding: var(--spacing-xs);
        }

        /* =========================================================
           MAIN LAYOUT WITH SIDEBAR
        ========================================================= */
        .main-layout {
            display: flex;
            flex: 1;
            position: relative;
        }

        /* Sidebar */
        .sidebar {
            width: var(--sidebar-width);
            position: sticky;
            top: calc(var(--header-height) + var(--nav-height));
            height: calc(100vh - calc(var(--header-height) + var(--nav-height)));
            overflow-y: auto;
            background: var(--surface);
            border-right: 1px solid var(--border);
            padding: var(--spacing-lg);
            direction: rtl;
            text-align: right;
        }

        .sidebar-header {
            margin-bottom: var(--spacing-xl);
            padding-bottom: var(--spacing-md);
            border-bottom: 2px solid var(--primary);
            text-align: center;
        }

        .sidebar-header h3 {
            color: var(--primary);
            font-size: var(--font-size-xl);
            margin-bottom: var(--spacing-xs);
        }

        .sidebar-header p {
            font-size: var(--font-size-sm);
            color: var(--text-light);
        }

        .sidebar-section {
            margin-bottom: var(--spacing-xl);
        }

        .sidebar-section h4 {
            font-size: var(--font-size-base);
            color: var(--primary-dark);
            margin-bottom: var(--spacing-sm);
            padding-right: var(--spacing-sm);
            position: relative;
        }

        .sidebar-section h4::before {
            content: '▼';
            position: absolute;
            left: 0;
            color: var(--primary);
        }

        .disability-types {
            display: flex;
            flex-direction: column;
            gap: var(--spacing-xs);
        }

        .disability-type {
            padding: var(--spacing-sm) var(--spacing-md);
            border-radius: var(--radius);
            background: var(--surface);
            border: 1px solid var(--border);
            transition: var(--transition-fast);
            cursor: pointer;
            display: flex;
            align-items: center;
            gap: var(--spacing-sm);
            text-align: right;
        }

        .disability-type:hover,
        .disability-type:focus {
            background: var(--primary-light);
            border-color: var(--primary);
            transform: translateX(-3px);
        }

        .disability-type.active {
            background: var(--primary);
            color: white;
            border-color: var(--primary);
        }

        .disability-type-icon {
            font-size: 1.2rem;
        }

        .disability-type span {
            font-weight: 600;
            font-size: var(--font-size-sm);
        }

        .sidebar-nav ul {
            list-style: none;
        }

        .sidebar-nav li {
            margin-bottom: var(--spacing-xs);
        }

        .sidebar-nav a {
            display: block;
            padding: var(--spacing-sm) var(--spacing-md);
            border-radius: var(--radius);
            font-size: var(--font-size-sm);
            transition: var(--transition-fast);
            color: var(--text);
        }

        .sidebar-nav a:hover,
        .sidebar-nav a:focus {
            background: var(--surface-soft);
            color: var(--primary);
        }

        /* Content Area */
        .content-area {
            flex: 1;
            padding: var(--spacing-xl);
            min-width: 0;
        }

        /* =========================================================
           HERO SECTION
        ========================================================= */
        .hero {
            background: var(--surface);
            border-radius: var(--radius-xl);
            padding: var(--spacing-2xl);
            margin-bottom: var(--spacing-xl);
            box-shadow: var(--shadow);
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, rgba(7, 89, 133, 0.1), rgba(14, 165, 233, 0.05));
            z-index: 0;
        }

        .hero-content {
            position: relative;
            z-index: 1;
        }

        .hero h1 {
            color: var(--primary);
            font-size: clamp(var(--font-size-2xl), 4vw, var(--font-size-3xl));
            font-weight: 800;
            margin-bottom: var(--spacing-md);
            line-height: 1.3;
        }

        .hero p {
            color: var(--text-soft);
            font-size: var(--font-size-lg);
            max-width: 800px;
            margin-bottom: var(--spacing-lg);
        }

        .hero-slogan {
            font-size: var(--font-size-xl);
            font-weight: 700;
            color: var(--primary-dark);
            margin-bottom: var(--spacing-lg);
            display: flex;
            align-items: center;
            gap: var(--spacing-sm);
        }

        .hero-slogan .gem-icon {
            font-size: 1.5rem;
            color: var(--gold);
        }

        .cta-buttons {
            display: flex;
            gap: var(--spacing-md);
            justify-content: flex-start;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: var(--spacing-xs);
            padding: var(--spacing-sm) var(--spacing-lg);
            border-radius: var(--radius-lg);
            font-weight: 700;
            font-size: var(--font-size-base);
            transition: var(--transition);
            border: none;
            cursor: pointer;
            text-decoration: none;
        }

        .btn-primary {
            background: var(--gold);
            color: var(--primary-dark);
        }

        .btn-primary:hover,
        .btn-primary:focus {
            background: var(--gold-dark);
            transform: translateY(-2px);
            box-shadow: var(--shadow);
        }

        .btn-secondary {
            background: var(--surface);
            color: var(--primary);
            border: 2px solid var(--primary);
        }

        .btn-secondary:hover,
        .btn-secondary:focus {
            background: var(--primary);
            color: white;
        }

        /* =========================================================
           SECTIONS
        ========================================================= */
        .section {
            margin-bottom: var(--spacing-xl);
        }

        .section-title {
            text-align: right;
            margin-bottom: var(--spacing-xl);
            position: relative;
        }

        .section-title h2 {
            color: var(--primary);
            font-size: clamp(var(--font-size-xl), 3vw, var(--font-size-3xl));
            font-weight: 800;
            margin-bottom: var(--spacing-sm);
        }

        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: linear-gradient(90deg, var(--primary), var(--gold));
            margin-top: var(--spacing-sm);
            border-radius: 2px;
        }

        .section-subtitle {
            color: var(--text-soft);
            font-size: var(--font-size-lg);
            max-width: 800px;
        }

        /* =========================================================
           CARDS
        ========================================================= */
        .cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: var(--spacing-lg);
        }

        .card {
            background: var(--surface);
            border: 1px solid var(--border);
            border-radius: var(--radius-xl);
            padding: var(--spacing-lg);
            transition: var(--transition);
            box-shadow: var(--shadow-sm);
        }

        .card:hover,
        .card:focus-within {
            transform: translateY(-5px);
            box-shadow: var(--shadow-lg);
            border-color: var(--primary);
        }

        .card-icon {
            width: 60px;
            height: 60px;
            background: linear-gradient(135deg, var(--primary), var(--primary-light));
            border-radius: var(--radius-full);
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: var(--spacing-md);
            font-size: 1.8rem;
            color: white;
        }

        .card h3 {
            color: var(--primary);
            font-size: var(--font-size-lg);
            margin-bottom: var(--spacing-sm);
        }

        .card p {
            color: var(--text-light);
            font-size: var(--font-size-base);
            margin-bottom: 0;
        }

        /* =========================================================
           ABOUT SECTION
        ========================================================= */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: var(--spacing-xl);
            align-items: center;
        }

        .about-image {
            width: 100%;
            height: 400px;
            object-fit: cover;
            border-radius: var(--radius-xl);
            border: 5px solid var(--primary);
            box-shadow: var(--shadow);
        }

        .about-text h3 {
            color: var(--primary);
            font-size: var(--font-size-xl);
            margin-bottom: var(--spacing-md);
        }

        .about-text p {
            margin-bottom: var(--spacing-md);
            color: var(--text-light);
            font-size: var(--font-size-base);
            line-height: 2;
        }

        .about-text blockquote {
            border-right: 4px solid var(--gold);
            padding-right: var(--spacing-md);
            margin: var(--spacing-lg) 0;
            color: var(--primary-dark);
            font-style: italic;
            font-size: var(--font-size-lg);
            font-weight: 600;
        }

        /* =========================================================
           DISABILITY CONTENT
        ========================================================= */
        .disability-content {
            display: none;
        }

        .disability-content.active {
            display: block;
            animation: fadeIn 0.5s ease;
        }

        .disability-detail {
            background: var(--surface);
            border: 1px solid var(--border);
            border-radius: var(--radius-xl);
            padding: var(--spacing-xl);
            margin-bottom: var(--spacing-lg);
            box-shadow: var(--shadow-sm);
        }

        .disability-detail h3 {
            color: var(--primary);
            font-size: var(--font-size-xl);
            margin-bottom: var(--spacing-md);
            display: flex;
            align-items: center;
            gap: var(--spacing-sm);
        }

        .disability-features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: var(--spacing-md);
            margin-top: var(--spacing-md);
        }

        .feature-item {
            display: flex;
            align-items: flex-start;
            gap: var(--spacing-sm);
            padding: var(--spacing-sm);
            border-radius: var(--radius);
            background: var(--surface-soft);
        }

        .feature-icon {
            color: var(--primary);
            font-size: 1.2rem;
            margin-top: 2px;
        }

        /* =========================================================
           SERVICES SECTION
        ========================================================= */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: var(--spacing-lg);
        }

        .service-card {
            text-align: center;
            padding: var(--spacing-lg);
        }

        .service-icon {
            width: 80px;
            height: 80px;
            background: var(--surface-soft);
            border-radius: var(--radius-full);
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto var(--spacing-lg);
            font-size: 2.5rem;
            color: var(--primary);
            border: 3px solid var(--primary);
        }

        .service-card h3 {
            color: var(--primary);
            font-size: var(--font-size-lg);
            margin-bottom: var(--spacing-sm);
        }

        .service-card p {
            color: var(--text-light);
            font-size: var(--font-size-sm);
        }

        /* =========================================================
           CONTACT FORM
        ========================================================= */
        .contact-form {
            max-width: 700px;
            margin: 0 auto;
            background: var(--surface);
            padding: var(--spacing-xl);
            border-radius: var(--radius-xl);
            border: 1px solid var(--border);
            box-shadow: var(--shadow);
        }

        .form-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: var(--spacing-md);
        }

        .form-group {
            margin-bottom: var(--spacing-md);
        }

        .form-group label {
            display: block;
            margin-bottom: var(--spacing-xs);
            font-weight: 700;
            color: var(--text);
            font-size: var(--font-size-base);
        }

        .form-group label span {
            color: var(--danger);
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: var(--spacing-sm) var(--spacing-md);
            border: 2px solid var(--border);
            border-radius: var(--radius);
            font-family: inherit;
            font-size: var(--font-size-base);
            transition: var(--transition-fast);
            background: var(--surface);
            color: var(--text);
        }

        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(7, 89, 133, 0.1);
        }

        .form-group textarea {
            min-height: 150px;
            resize: vertical;
        }

        .form-group input::placeholder,
        .form-group textarea::placeholder {
            color: var(--text-muted);
        }

        .form-actions {
            display: flex;
            gap: var(--spacing-md);
            margin-top: var(--spacing-lg);
        }

        .form-actions .btn {
            flex: 1;
        }

        .consent {
            display: flex;
            align-items: flex-start;
            gap: var(--spacing-sm);
            padding: var(--spacing-md);
            margin: var(--spacing-md) 0;
            border-radius: var(--radius);
            background: var(--surface-soft);
            border: 1px solid var(--border);
        }

        .consent input {
            width: 18px;
            height: 18px;
            flex-shrink: 0;
            margin-top: 3px;
            accent-color: var(--primary);
        }

        .consent span {
            font-size: var(--font-size-sm);
            color: var(--text-soft);
            line-height: 1.8;
        }

        /* =========================================================
           CHATBOT
        ========================================================= */
        .chatbot-container {
            position: fixed;
            bottom: var(--spacing-lg);
            left: var(--spacing-lg);
            z-index: 1000;
            direction: rtl;
        }

        .chatbot-toggle {
            width: 60px;
            height: 60px;
            border-radius: var(--radius-full);
            background: var(--primary);
            color: white;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
            box-shadow: var(--shadow-lg);
            transition: var(--transition);
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .chatbot-toggle:hover {
            background: var(--primary-dark);
            transform: scale(1.1);
        }

        .chatbot-popup {
            position: absolute;
            bottom: calc(var(--spacing-lg) + 60px);
            left: 0;
            width: 350px;
            background: var(--surface);
            border-radius: var(--radius-xl);
            box-shadow: var(--shadow-lg);
            border: 1px solid var(--border);
            opacity: 0;
            visibility: hidden;
            transform: translateY(20px);
            transition: var(--transition);
            max-height: 500px;
            overflow-y: auto;
        }

        .chatbot-popup.active {
            opacity: 1;
            visibility: visible;
            transform: translateY(0);
        }

        .chatbot-header {
            background: var(--primary);
            color: white;
            padding: var(--spacing-md);
            border-top-right-radius: var(--radius-xl);
            border-top-left-radius: var(--radius-xl);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .chatbot-header h4 {
            font-size: var(--font-size-base);
            font-weight: 700;
            margin: 0;
        }

        .chatbot-close {
            background: none;
            border: none;
            color: white;
            font-size: 1.2rem;
            cursor: pointer;
            padding: var(--spacing-xs);
        }

        .chatbot-messages {
            padding: var(--spacing-md);
            max-height: 350px;
            overflow-y: auto;
        }

        .chatbot-message {
            margin-bottom: var(--spacing-md);
            padding: var(--spacing-sm) var(--spacing-md);
            border-radius: var(--radius);
            max-width: 85%;
            word-wrap: break-word;
        }

        .chatbot-message.user {
            background: var(--primary-light);
            color: white;
            margin-left: auto;
            border-bottom-right-radius: var(--radius-xs);
        }

        .chatbot-message.bot {
            background: var(--surface-soft);
            color: var(--text);
            margin-right: auto;
            border-bottom-left-radius: var(--radius-xs);
        }

        .chatbot-input-container {
            padding: var(--spacing-md);
            border-top: 1px solid var(--border);
            background: var(--surface-soft);
        }

        .chatbot-input {
            width: 100%;
            padding: var(--spacing-sm) var(--spacing-md);
            border: 2px solid var(--border);
            border-radius: var(--radius);
            font-size: var(--font-size-base);
            transition: var(--transition-fast);
        }

        .chatbot-input:focus {
            outline: none;
            border-color: var(--primary);
        }

        .chatbot-send {
            background: var(--primary);
            color: white;
            border: none;
            padding: var(--spacing-sm) var(--spacing-md);
            border-radius: var(--radius);
            margin-top: var(--spacing-sm);
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition-fast);
        }

        .chatbot-send:hover {
            background: var(--primary-dark);
        }

        .chatbot-typing {
            display: flex;
            gap: 5px;
            padding: 5px 0;
        }

        .chatbot-typing span {
            width: 8px;
            height: 8px;
            background: var(--text-light);
            border-radius: 50%;
            animation: typing 1.4s infinite ease-in-out;
        }

        .chatbot-typing span:nth-child(2) {
            animation-delay: 0.2s;
        }

        .chatbot-typing span:nth-child(3) {
            animation-delay: 0.4s;
        }

        @keyframes typing {
            0%, 60%, 100% {
                transform: translateY(0);
            }
            30% {
                transform: translateY(-5px);
            }
        }

        /* =========================================================
           GAME SECTION (from user's code)
        ========================================================= */
        .game-card {
            text-align: center;
        }

        .game-box {
            margin-top: var(--spacing-md);
            background: var(--surface-soft);
            border-radius: var(--radius-xl);
            padding: var(--spacing-xl);
        }

        .game-question {
            font-size: 2rem;
            font-weight: bold;
            margin-bottom: var(--spacing-lg);
            color: var(--text);
        }

        .game-options {
            display: flex;
            justify-content: center;
            gap: var(--spacing-md);
            flex-wrap: wrap;
        }

        .game-options button {
            min-width: 80px;
            min-height: 60px;
            font-size: 1.8rem;
            border: 2px solid var(--border);
            background: var(--surface);
            border-radius: var(--radius-lg);
            cursor: pointer;
            transition: var(--transition-fast);
        }

        .game-options button:hover {
            background: var(--surface-soft);
            border-color: var(--primary);
        }

        .game-message {
            margin-top: var(--spacing-md);
            font-weight: 700;
            min-height: 30px;
            font-size: var(--font-size-lg);
        }

        /* =========================================================
           VIDEO SECTION
        ========================================================= */
        .video-card {
            overflow: hidden;
        }

        .video-placeholder {
            height: 180px;
            border-radius: var(--radius-lg);
            background: linear-gradient(135deg, var(--primary), var(--primary-light));
            display: grid;
            place-items: center;
            color: white;
            font-size: 3rem;
        }

        .video-controls {
            display: flex;
            gap: var(--spacing-xs);
            margin-top: var(--spacing-sm);
            flex-wrap: wrap;
        }

        .video-controls button {
            border: none;
            background: var(--surface-soft);
            color: var(--text);
            padding: var(--spacing-xs) var(--spacing-sm);
            border-radius: var(--radius);
            font-size: var(--font-size-sm);
            cursor: pointer;
            transition: var(--transition-fast);
        }

        .video-controls button:hover {
            background: var(--primary);
            color: white;
        }

        /* =========================================================
           LIBRARY SECTION
        ========================================================= */
        .library-filter {
            display: flex;
            justify-content: center;
            gap: var(--spacing-xs);
            flex-wrap: wrap;
            margin-bottom: var(--spacing-xl);
        }

        .library-filter button {
            border: 1px solid var(--border);
            background: var(--surface);
            color: var(--text);
            padding: var(--spacing-xs) var(--spacing-md);
            border-radius: var(--radius);
            font-size: var(--font-size-sm);
            cursor: pointer;
            transition: var(--transition-fast);
        }

        .library-filter button.active,
        .library-filter button:hover {
            background: var(--primary);
            color: white;
            border-color: var(--primary);
        }

        .library-item {
            display: none;
        }

        .library-item.active {
            display: block;
        }

        /* =========================================================
           FOOTER
        ========================================================= */
        footer {
            background: var(--primary-bg);
            color: rgba(255, 255, 255, 0.8);
            padding: var(--spacing-2xl) var(--spacing-md) var(--spacing-xl);
            margin-top: auto;
        }

        .footer-container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: var(--spacing-xl);
        }

        .footer-section h3 {
            color: white;
            font-size: var(--font-size-xl);
            margin-bottom: var(--spacing-md);
        }

        .footer-section ul {
            list-style: none;
        }

        .footer-section ul li {
            margin-bottom: var(--spacing-xs);
        }

        .footer-section a {
            color: rgba(255, 255, 255, 0.8);
            display: block;
            padding: var(--spacing-xs) 0;
        }

        .footer-section a:hover,
        .footer-section a:focus {
            color: var(--gold);
        }

        .footer-section p {
            margin-bottom: var(--spacing-xs);
            color: rgba(255, 255, 255, 0.7);
        }

        .footer-bottom {
            max-width: 1400px;
            margin: var(--spacing-xl) auto 0;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            padding-top: var(--spacing-lg);
            text-align: center;
        }

        .footer-bottom p {
            color: rgba(255, 255, 255, 0.6);
            font-size: var(--font-size-sm);
        }

        /* =========================================================
           TOAST NOTIFICATION
        ========================================================= */
        .toast {
            position: fixed;
            bottom: var(--spacing-xl);
            right: var(--spacing-xl);
            background: var(--primary-dark);
            color: white;
            padding: var(--spacing-md) var(--spacing-lg);
            border-radius: var(--radius-lg);
            transform: translateY(120px);
            opacity: 0;
            transition: var(--transition);
            z-index: 3000;
            box-shadow: var(--shadow-lg);
        }

        .toast.show {
            transform: translateY(0);
            opacity: 1;
        }

        /* =========================================================
           RESPONSIVE DESIGN
        ========================================================= */
        @media (max-width: 1200px) {
            .main-layout {
                flex-direction: column;
            }

            .sidebar {
                width: 100%;
                position: relative;
                top: 0;
                height: auto;
                border-right: none;
                border-bottom: 1px solid var(--border);
                order: 2;
            }

            .content-area {
                order: 1;
            }

            .about-content {
                grid-template-columns: 1fr;
            }

            .about-image {
                height: 350px;
                margin: var(--spacing-lg) auto;
            }

            .form-grid {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 992px) {
            .top-header-container {
                flex-direction: column;
                gap: var(--spacing-sm);
                text-align: center;
            }

            .header-nav {
                justify-content: center;
                width: 100%;
            }

            .nav-container {
                flex-direction: column;
                gap: var(--spacing-sm);
                text-align: center;
            }

            .nav-links {
                justify-content: center;
            }

            .mobile-menu-btn {
                display: block;
            }

            .nav-links {
                display: none;
                flex-direction: column;
                position: absolute;
                top: 100%;
                right: 0;
                background: var(--surface);
                width: 100%;
                padding: var(--spacing-md);
                box-shadow: var(--shadow);
            }

            .nav-links.active {
                display: flex;
            }

            .hero {
                padding: var(--spacing-xl);
            }

            .hero h1 {
                font-size: var(--font-size-2xl);
            }

            .cta-buttons {
                flex-direction: column;
                align-items: flex-start;
            }

            .disability-types {
                display: grid;
                grid-template-columns: 1fr 1fr;
                gap: var(--spacing-xs);
            }

            .chatbot-container {
                left: var(--spacing-md);
                bottom: var(--spacing-md);
            }

            .chatbot-popup {
                width: calc(100% - var(--spacing-lg));
                max-width: 350px;
            }
        }

        @media (max-width: 768px) {
            :root {
                --header-height: 180px;
                --nav-height: 50px;
            }

            .top-header {
                padding: var(--spacing-sm);
            }

            .header-logo-text .institute {
                font-size: var(--font-size-xs);
            }

            .header-logo-text .center {
                font-size: var(--font-size-base);
            }

            .header-nav {
                display: none;
            }

            .slider-container {
                height: var(--header-height);
            }

            .main-nav {
                top: var(--header-height);
            }

            .main-layout {
                flex-direction: column;
            }

            .sidebar {
                position: fixed;
                top: calc(var(--header-height) + var(--nav-height));
                right: -100%;
                width: var(--sidebar-width);
                height: calc(100vh - calc(var(--header-height) + var(--nav-height)));
                transition: right var(--transition);
                z-index: 998;
            }

            .sidebar.active {
                right: 0;
            }

            .content-area {
                margin-right: 0;
            }

            .hero {
                padding: var(--spacing-lg);
            }

            .hero h1 {
                font-size: var(--font-size-xl);
            }

            .hero p {
                font-size: var(--font-size-base);
            }

            .section-title h2 {
                font-size: var(--font-size-xl);
            }

            .disability-types {
                grid-template-columns: 1fr;
            }

            .cards-grid {
                grid-template-columns: 1fr;
            }

            .services-grid {
                grid-template-columns: 1fr;
            }

            .form-grid {
                grid-template-columns: 1fr;
            }

            .accessibility-bar {
                font-size: var(--font-size-xs);
                padding: var(--spacing-xs);
            }

            .accessibility-bar button {
                padding: var(--spacing-xs);
                font-size: var(--font-size-xs);
            }
        }

        @media (max-width: 480px) {
            .container {
                padding: 0 var(--spacing-sm);
            }

            .header-logo-icon {
                width: 40px;
                height: 40px;
                font-size: 1.3rem;
            }

            .header-logo-text .center {
                font-size: var(--font-size-sm);
            }

            .nav-logo-icon {
                width: 35px;
                height: 35px;
            }

            .hero h1 {
                font-size: var(--font-size-lg);
            }

            .btn {
                padding: var(--spacing-xs) var(--spacing-md);
                font-size: var(--font-size-sm);
            }

            .chatbot-toggle {
                width: 50px;
                height: 50px;
                font-size: 1.2rem;
            }

            .chatbot-popup {
                width: calc(100% - var(--spacing-md));
            }

            .toast {
                right: var(--spacing-md);
                bottom: var(--spacing-md);
                padding: var(--spacing-sm) var(--spacing-md);
            }
        }

        /* =========================================================
           ANIMATIONS
        ========================================================= */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes slideIn {
            from { transform: translateX(100%); }
            to { transform: translateX(0); }
        }

        .card,
        .service-card,
        .disability-detail,
        .testimonial {
            animation: fadeIn 0.6s ease forwards;
        }

        /* =========================================================
           REDUCED MOTION
        ========================================================= */
        @media (prefers-reduced-motion: reduce) {
            *,
            *::before,
            *::after {
                animation-duration: 0.01ms !important;
                animation-iteration-count: 1 !important;
                transition-duration: 0.01ms !important;
            }

            .slider {
                transition: none !important;
            }
        }

        /* =========================================================
           PRINT STYLES
        ========================================================= */
        @media print {
            .top-header,
            .accessibility-bar,
            .main-nav,
            .sidebar,
            .chatbot-container,
            .toast {
                display: none !important;
            }

            body {
                background: white;
                color: black;
            }

            .main-layout {
                display: block;
            }

            .section {
                page-break-inside: avoid;
            }
        }

        /* =========================================================
           CUSTOM SCROLLBAR
        ========================================================= */
        ::-webkit-scrollbar {
            width: 8px;
            height: 8px;
        }

        ::-webkit-scrollbar-track {
            background: var(--surface-soft);
        }

        ::-webkit-scrollbar-thumb {
            background: var(--primary);
            border-radius: 4px;
        }

        ::-webkit-scrollbar-thumb:hover {
            background: var(--primary-dark);
        }

        /* =========================================================
           SIDEBAR TOGGLE BUTTON
        ========================================================= */
        .sidebar-toggle {
            display: none;
            position: fixed;
            top: calc(var(--header-height) + var(--nav-height) + 10px);
            right: var(--spacing-md);
            z-index: 999;
            background: var(--primary);
            color: white;
            border: none;
            padding: var(--spacing-xs) var(--spacing-md);
            border-radius: var(--radius);
            font-weight: 600;
            font-size: var(--font-size-sm);
            cursor: pointer;
            transition: var(--transition-fast);
        }

        .sidebar-toggle:hover {
            background: var(--primary-dark);
        }

        @media (max-width: 992px) {
            .sidebar-toggle {
                display: block;
            }
        }

        /* =========================================================
           NEGIN CONTACT FORM STYLES
        ========================================================= */
        .negin-contact-section {
            width: min(950px, calc(100% - 30px));
            margin: 60px auto;
            padding: 45px 30px;
            background: var(--surface);
            border-radius: var(--radius-xl);
            border: 1px solid var(--border);
            box-shadow: var(--shadow-lg);
            direction: rtl;
        }

        .negin-contact-header {
            text-align: center;
            margin-bottom: 35px;
        }

        .negin-contact-badge {
            display: inline-block;
            padding: 8px 16px;
            border-radius: 50px;
            background: var(--surface-soft);
            color: var(--primary);
            font-weight: 800;
            font-size: 13px;
            margin-bottom: 15px;
        }

        .negin-contact-header h2 {
            margin: 0 0 12px;
            color: var(--primary-dark);
            font-size: clamp(24px, 4vw, 34px);
            font-weight: 900;
        }

        .negin-contact-header p {
            max-width: 700px;
            margin: auto;
            color: var(--text-soft);
            line-height: 2;
            font-size: 15px;
        }

        .negin-contact-form {
            width: 100%;
        }

        .negin-form-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
        }

        .negin-form-group {
            margin-bottom: 20px;
        }

        .negin-form-group label {
            display: block;
            margin-bottom: 8px;
            color: var(--text);
            font-weight: 800;
            font-size: 14px;
        }

        .negin-form-group label span {
            color: var(--danger);
        }

        .negin-form-group input,
        .negin-form-group select,
        .negin-form-group textarea {
            width: 100%;
            border: 1px solid var(--border);
            border-radius: var(--radius-lg);
            background: var(--surface);
            color: var(--text);
            padding: 13px 15px;
            font-family: inherit;
            font-size: 14px;
            outline: none;
            transition: var(--transition-fast);
        }

        .negin-form-group input,
        .negin-form-group select {
            height: 52px;
        }

        .negin-form-group textarea {
            resize: vertical;
            min-height: 150px;
            line-height: 2;
        }

        .negin-form-group input:focus,
        .negin-form-group select:focus,
        .negin-form-group textarea:focus {
            border-color: var(--primary-light);
            box-shadow: 0 0 0 4px rgba(14, 165, 233, .12);
        }

        .negin-form-group input::placeholder,
        .negin-form-group textarea::placeholder {
            color: var(--text-muted);
        }

        .negin-consent {
            display: flex;
            align-items: flex-start;
            gap: 10px;
            padding: 15px;
            margin: 5px 0 20px;
            border-radius: var(--radius-lg);
            background: var(--surface-soft);
            border: 1px solid var(--border-strong);
            color: var(--text-soft);
            font-size: 13px;
            line-height: 1.9;
            cursor: pointer;
        }

        .negin-consent input {
            width: 19px;
            height: 19px;
            flex: 0 0 19px;
            margin-top: 3px;
            accent-color: var(--primary);
        }

        .negin-submit {
            width: 100%;
            min-height: 56px;
            border: 1px solid var(--gold-dark);
            border-radius: var(--radius);
            background: var(--gold);
            color: #111111;
            font-family: inherit;
            font-size: 16px;
            font-weight: 900;
            cursor: pointer;
            transition: var(--transition-fast);
        }

        .negin-submit:hover {
            background: var(--gold-dark);
            transform: translateY(-2px);
            box-shadow: 0 12px 30px rgba(201, 157, 0, .20);
        }

        .negin-submit:active {
            transform: scale(.98);
        }

        .negin-email-note {
            text-align: center;
            margin: 18px 0 0;
            color: var(--text-light);
            font-size: 12px;
            line-height: 1.8;
        }

        .negin-email-note strong {
            color: var(--primary);
            direction: ltr;
            display: inline-block;
        }

        /* Negin Contact Form - Mobile */
        @media (max-width: 650px) {
            .negin-contact-section {
                width: calc(100% - 20px);
                margin: 35px auto;
                padding: 30px 17px;
                border-radius: var(--radius-xl);
            }

            .negin-form-grid {
                grid-template-columns: 1fr;
                gap: 0;
            }

            .negin-contact-header h2 {
                font-size: 23px;
            }

            .negin-contact-header p {
                font-size: 13px;
            }

            .negin-form-group input,
            .negin-form-group select {
                height: 50px;
            }

            .negin-submit {
                min-height: 54px;
                font-size: 15px;
            }
        }

        /* Negin Contact Form - Dark Mode */
        body.dark .negin-contact-section {
            background: var(--surface);
            border-color: var(--border);
        }

        body.dark .negin-contact-badge {
            background: var(--surface-soft);
            color: var(--primary-light);
        }

        body.dark .negin-contact-header h2,
        body.dark .negin-form-group label {
            color: var(--text);
        }

        body.dark .negin-contact-header p,
        body.dark .negin-consent,
        body.dark .negin-email-note {
            color: var(--text-soft);
        }

        body.dark .negin-form-group input,
        body.dark .negin-form-group select,
        body.dark .negin-form-group textarea {
            background: var(--surface);
            color: var(--text);
            border-color: var(--border);
        }

        body.dark .negin-consent {
            background: var(--surface-soft);
            border-color: var(--border);
        }

        /* Negin Contact Form - High Contrast */
        body.high-contrast .negin-contact-section,
        body.high-contrast .negin-form-group input,
        body.high-contrast .negin-form-group select,
        body.high-contrast .negin-form-group textarea,
        body.high-contrast .negin-consent {
            border: 2px solid var(--text);
            box-shadow: none;
        }

        body.high-contrast .negin-contact-header h2,
        body.high-contrast .negin-contact-header p,
        body.high-contrast .negin-form-group label,
        body.high-contrast .negin-email-note {
            color: var(--text);
        }

        /* =========================================================
           ACCORDION STYLES
        ========================================================= */
        .accordion-container {
            display: flex;
            flex-direction: column;
            gap: var(--spacing-md);
            margin-top: var(--spacing-lg);
        }

        .accordion-item {
            border: 1px solid var(--border);
            border-radius: var(--radius-lg);
            background: var(--surface);
            overflow: hidden;
            box-shadow: var(--shadow-sm);
            transition: var(--transition);
        }

        .accordion-item:focus-within {
            border-color: var(--primary);
            box-shadow: 0 0 0 4px rgba(7, 89, 133, 0.1);
        }

        .accordion-header {
            width: 100%;
            display: flex;
            align-items: center;
            gap: var(--spacing-sm);
            padding: var(--spacing-md) var(--spacing-lg);
            background: var(--surface);
            border: none;
            cursor: pointer;
            text-align: right;
            font-family: inherit;
            transition: var(--transition);
        }

        .accordion-header:hover {
            background: var(--surface-soft);
        }

        .accordion-icon {
            font-size: 1.5rem;
            flex-shrink: 0;
        }

        .accordion-title {
            flex: 1;
            font-size: var(--font-size-lg);
            font-weight: 700;
            color: var(--primary-dark);
            text-align: right;
        }

        .accordion-arrow {
            font-size: 1rem;
            color: var(--primary);
            transition: var(--transition);
            flex-shrink: 0;
        }

        .accordion-item[aria-expanded="true"] .accordion-arrow {
            transform: rotate(180deg);
        }

        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.4s ease;
            padding: 0 var(--spacing-lg);
        }

        .accordion-content[hidden] {
            display: none;
        }

        .accordion-item[aria-expanded="true"] .accordion-content {
            max-height: 2000px;
            padding: var(--spacing-lg);
            border-top: 1px solid var(--border);
        }

        .accordion-body {
            display: flex;
            flex-direction: column;
            gap: var(--spacing-lg);
        }

        .accordion-body .lead {
            font-size: var(--font-size-lg);
            color: var(--text-soft);
            font-weight: 600;
            line-height: 1.8;
        }

        .accordion-body h4 {
            color: var(--primary);
            font-size: var(--font-size-xl);
            font-weight: 800;
            margin-bottom: var(--spacing-sm);
        }

        .accordion-body h5 {
            color: var(--primary-dark);
            font-size: var(--font-size-base);
            font-weight: 700;
            margin-bottom: var(--spacing-xs);
        }

        .accordion-body p {
            color: var(--text-soft);
            line-height: 1.9;
            font-size: var(--font-size-base);
        }

        .accordion-body ul {
            padding-right: var(--spacing-md);
            margin-bottom: var(--spacing-md);
        }

        .accordion-body li {
            color: var(--text-light);
            margin-bottom: var(--spacing-xs);
            line-height: 1.8;
        }

        /* Grid Layouts */
        .grid-2 {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: var(--spacing-md);
        }

        .method-grid,
        .assessment-grid,
        .activity-cards,
        .feature-cards {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
            gap: var(--spacing-md);
            margin: var(--spacing-md) 0;
        }

        .method-card,
        .assessment-item,
        .activity-card,
        .feature-card {
            background: var(--surface-soft);
            border: 1px solid var(--border);
            border-radius: var(--radius);
            padding: var(--spacing-md);
            text-align: center;
            transition: var(--transition);
        }

        .method-card:hover,
        .assessment-item:hover,
        .activity-card:hover,
        .feature-card:hover {
            background: var(--primary-light);
            border-color: var(--primary);
            transform: translateY(-3px);
            box-shadow: var(--shadow);
        }

        .method-icon,
        .assessment-icon,
        .activity-icon,
        .feature-icon {
            font-size: 1.8rem;
            display: block;
            margin-bottom: var(--spacing-xs);
        }

        .info-box {
            background: linear-gradient(135deg, rgba(7, 89, 133, 0.1), rgba(14, 165, 233, 0.05));
            border-left: 4px solid var(--gold);
            padding: var(--spacing-md) var(--spacing-lg);
            border-radius: var(--radius);
            margin-top: var(--spacing-md);
        }

        .info-box p {
            margin: 0;
            color: var(--text);
            font-size: var(--font-size-base);
            line-height: 1.9;
        }

        .info-box strong {
            color: var(--primary-dark);
        }

        .info-box ul {
            padding-right: var(--spacing-sm);
            margin-top: var(--spacing-sm);
        }

        /* Dark Mode for Accordion */
        body.dark .accordion-item {
            background: var(--surface);
            border-color: var(--border);
        }

        body.dark .accordion-header:hover {
            background: var(--surface-soft);
        }

        body.dark .method-card,
        body.dark .assessment-item,
        body.dark .activity-card,
        body.dark .feature-card {
            background: var(--surface-soft);
            border-color: var(--border);
        }

        body.dark .method-card:hover,
        body.dark .assessment-item:hover,
        body.dark .activity-card:hover,
        body.dark .feature-card:hover {
            background: var(--primary-dark);
            border-color: var(--primary);
        }

        body.dark .info-box {
            background: linear-gradient(135deg, rgba(7, 89, 133, 0.2), rgba(14, 165, 233, 0.1));
        }

        /* High Contrast Mode for Accordion */
        body.high-contrast .accordion-item {
            border: 2px solid var(--text);
        }

        body.high-contrast .accordion-header {
            border-bottom: 1px solid var(--text);
        }

        body.high-contrast .method-card,
        body.high-contrast .assessment-item,
        body.high-contrast .activity-card,
        body.high-contrast .feature-card {
            border: 2px solid var(--text);
        }

        body.high-contrast .info-box {
            border-left: 4px solid var(--text);
        }

        /* Accordion Mobile */
        @media (max-width: 768px) {
            .grid-2 {
                grid-template-columns: 1fr;
            }

            .method-grid,
            .assessment-grid,
            .activity-cards,
            .feature-cards {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 480px) {
            .method-grid,
            .assessment-grid,
            .activity-cards,
            .feature-cards {
                grid-template-columns: 1fr;
            }
        }

        /* =========================================================
    <!-- Load Persian Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@100;200;300;400;500;600;700;800;900&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Arabic:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <!-- =====================================================
         IMAGE SLIDER (Background)
    ===================================================== -->
    <div class="slider-container">
        <div class="slider" id="imageSlider">
            <div class="slide">
                <img src="../../../uploads/1000004261.jpg" alt="کودک در کلاس آموزشی مرکز نگین" loading="lazy">
                <div class="slide-overlay"></div>
            </div>
            <div class="slide">
                <img src="https://images.unsplash.com/photo-1559757148-5c350d0d3c56?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80" alt="کودکان دارای معلولیت در حال فعالیت">
                <div class="slide-overlay"></div>
            </div>
            <div class="slide">
                <img src="https://images.unsplash.com/photo-1544717297-fa95b6ee9643?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80" alt="کودک دارای اوتیسم در کلاس">
                <div class="slide-overlay"></div>
            </div>
            <div class="slide">
                <img src="https://images.unsplash.com/photo-1559839734-2b71ea197ec2?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80" alt="درمانگر در حال کار با کودک">
                <div class="slide-overlay"></div>
            </div>
            <div class="slide">
                <img src="https://images.unsplash.com/photo-1594736797933-d0401ba2fe65?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80" alt="کودک نابینا با عصا">
                <div class="slide-overlay"></div>
            </div>
            <div class="slide">
                <img src="https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80" alt="کودکان در حال استفاده از زبان اشاره">
                <div class="slide-overlay"></div>
            </div>
            <div class="slide">
                <img src="https://images.unsplash.com/photo-1604467795338-03f232406a2b?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80" alt="کودک در حال فیزیوتراپی">
                <div class="slide-overlay"></div>
            </div>
            <div class="slide">
                <img src="https://images.unsplash.com/photo-1503454537195-1dcabb73ffb9?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80" alt="کلاس آموزشی ویژه کودکان">
                <div class="slide-overlay"></div>
            </div>
        </div>
        <div class="slider-dots" id="sliderDots"></div>
    </div>

    <!-- =====================================================
         TOP HEADER - مؤسسه نگین
    ===================================================== -->
    <header class="top-header">
        <div class="top-header-container">
            <div class="header-logo">
                <img src="../../../uploads/1000004238.png" alt="مرکز آموزشی و توان‌بخشی نگین" class="header-logo-img" loading="lazy">
                <div class="header-logo-text">
                    <span class="institute">مؤسسه‌ی خدماتی و حرفه‌ای زنان بی‌بضاعت</span>
                    <span class="center">مرکز آموزشی و توان‌بخشی نگین</span>
                    <span class="slogan">«هر کودک، یک نگین» <span class="gem">💎</span></span>
                </div>
            </div>
            <nav class="header-nav" aria-label="منوی اصلی">
                <a href="#home">خانه</a>
                <a href="#about">درباره نگین</a>
                <a href="#services">خدمات</a>
                <a href="#education">آموزش</a>
                <a href="#contact">تماس با ما</a>
            </nav>
        </div>
    </header>

    <!-- =====================================================
         ACCESSIBILITY BAR
    ===================================================== -->
    <div class="accessibility-bar" role="region" aria-label="نوار دسترسی‌پذیری">
        <strong>دسترس‌پذیری:</strong>
        <button onclick="increaseText()" aria-label="بزرگ‌نمایی متن">A+</button>
        <button onclick="decreaseText()" aria-label="کوچک‌نمایی متن">A-</button>
        <button onclick="resetText()" aria-label="اندازه اصلی متن">A</button>
        <button onclick="toggleDark()" aria-label="حالت تیره">🌙</button>
        <button onclick="toggleContrast()" aria-label="کنتراست بالا">◐</button>
    </div>

    <!-- =====================================================
         MAIN NAVIGATION
    ===================================================== -->
    <nav class="main-nav">
        <div class="nav-container">
            <a href="#home" class="nav-logo">
                <img src="../../../uploads/1000004238.png" alt="نگین" class="nav-logo-img" loading="lazy">
                <span class="nav-logo-text">نگین</span>
            </a>
            <button class="mobile-menu-btn" aria-label="منوی موبایل" aria-expanded="false" aria-controls="nav-links">
                ☰
            </button>
            <div class="nav-links" id="nav-links">
                <a href="#home">خانه</a>
                <a href="#about">درباره ما</a>
                <a href="#story">داستان نگین</a>
                <a href="#services">خدمات</a>
                <a href="#education">آموزش</a>
                <a href="#team">تیم ما</a>
                <a href="#contact">تماس</a>
            </div>
        </div>
    </nav>

    <!-- =====================================================
         MAIN LAYOUT WITH SIDEBAR
    ===================================================== -->
    <div class="main-layout">
        <!-- SIDEBAR -->
        <aside class="sidebar" id="sidebar">
            <div class="sidebar-header">
                <h3>انواع معلولیت</h3>
                <p>برای مشاهده اطلاعات هر نوع، روی آن کلیک کنید</p>
            </div>

            <div class="sidebar-section">
                <h4>دسته‌بندی‌ها</h4>
                <div class="disability-types" role="navigation" aria-label="انواع معلولیت">
                    <button class="disability-type active" data-target="physical" aria-current="true">
                        <span class="disability-type-icon">🦽</span>
                        <span>معلولیت جسمی و حرکتی</span>
                    </button>
                    <button class="disability-type" data-target="visual">
                        <span class="disability-type-icon">👁️</span>
                        <span>معلولیت بینایی</span>
                    </button>
                    <button class="disability-type" data-target="hearing">
                        <span class="disability-type-icon">👂</span>
                        <span>معلولیت شنوایی</span>
                    </button>
                    <button class="disability-type" data-target="speech">
                        <span class="disability-type-icon">🗣️</span>
                        <span>مشکلات گفتاری و ارتباطی</span>
                    </button>
                    <button class="disability-type" data-target="learning">
                        <span class="disability-type-icon">🧠</span>
                        <span>مشکلات یادگیری</span>
                    </button>
                    <button class="disability-type" data-target="developmental">
                        <span class="disability-type-icon">👶</span>
                        <span>اختلالات رشدی و نیازهای آموزشی ویژه</span>
                    </button>
                    <button class="disability-type" data-target="multiple">
                        <span class="disability-type-icon">🔄</span>
                        <span>معلولیت‌های چندگانه</span>
                    </button>
                    <button class="disability-type" data-target="supportive">
                        <span class="disability-type-icon">🤝</span>
                        <span>نیازهای حمایتی و آموزشی ویژه</span>
                    </button>
                </div>
            </div>

            <div class="sidebar-section">
                <h4>لینک‌های سریع</h4>
                <nav class="sidebar-nav" aria-label="لینک‌های سریع">
                    <ul>
                        <li><a href="#about">درباره موسسه</a></li>
                        <li><a href="#services">خدمات ما</a></li>
                        <li><a href="#education">بخش آموزش</a></li>
                        <li><a href="#games">بازی‌ها</a></li>
                        <li><a href="#videos">ویدیوها</a></li>
                        <li><a href="#library">کتابخانه</a></li>
                        <li><a href="#contact">تماس با ما</a></li>
                    </ul>
                </nav>
            </div>

            <div class="sidebar-section">
                <h4>ارتباط با ما</h4>
                <div style="display: flex; gap: 10px; justify-content: flex-start;">
                    <a href="tel:0786838002" style="color: var(--primary); font-size: 1.3rem;" aria-label="تماس تلفنی">📞</a>
                    <a href="mailto:negineducationcenter@gmail.com" style="color: var(--primary); font-size: 1.3rem;" aria-label="ارسال ایمیل">✉️</a>
                    <a href="https://maps.app.goo.gl/UTwdrbUfqR6ewS9D9" style="color: var(--primary); font-size: 1.3rem;" aria-label="موقعیت در نقشه">🗺️</a>
                </div>
            </div>
        </aside>

        <!-- CONTENT AREA -->
        <main id="main-content" class="content-area">
            <!-- HERO SECTION -->
            <section id="home" class="hero" aria-labelledby="hero-heading">
                <div class="hero-content">
                    <h1 id="hero-heading">مرکز آموزشی و توان‌بخشی نگین</h1>
                    <p>مؤسسه‌ی خدماتی و حرفه‌ای زنان بی‌بضاعت - «هر کودک، یک نگین» 💎</p>
                    <p class="hero-slogan">
                        <span>آموزش، توان‌بخشی و حمایت از کودکان دارای معلولیت</span>
                        <span class="gem-icon">💎</span>
                    </p>
                    <div class="cta-buttons">
                        <a href="#about" class="btn btn-primary">درباره ما</a>
                        <a href="#contact" class="btn btn-secondary">تماس با ما</a>
                    </div>
                </div>
            </section>

            <!-- ABOUT NEGIN SECTION -->
            <section id="about" class="section" aria-labelledby="about-heading">
                <div class="section-title">
                    <h2 id="about-heading">دربارهٔ ما</h2>
                    <p class="section-subtitle">ما نگین هستیم</p>
                </div>
                <div class="about-content">
                    <div class="about-text">
                        <p>
                            مرکز آموزشی و توان‌بخشی نگین با هدف آموزش، توان‌بخشی و حمایت از کودکان دارای معلولیت و نیازهای آموزشی ویژه در کابل ایجاد شده است.
                        </p>
                        <p>
                            این مرکز ثمرهٔ سال‌ها تلاش و دلسوزی <strong>اسدالله حیدری</strong> و <strong>ساحل حیدری</strong> و همراهی ارزشمند <strong>اجمیر خان میرزاد</strong> است؛ تلاشی برای ایجاد محیطی امن که در آن کودکان فرصت آموزش، رشد، ارتباط و شکوفایی توانایی‌های خود را داشته باشند.
                        </p>
                        <blockquote>
                            ما باور داریم که تفاوت، دلیل محرومیت نیست و هر کودک شایستهٔ فرصت، احترام و زندگی باکرامت است.
                        </blockquote>
                    </div>
                    <div>
                        <img src="https://images.unsplash.com/photo-1559839734-2b71ea197ec2?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" 
                             alt="تیم مرکز آموزشی و توان‌بخشی نگین" 
                             class="about-image" 
                             loading="lazy">
                    </div>
                </div>
            </section>

            <!-- STORY SECTION -->
            <section id="story" class="section" aria-labelledby="story-heading">
                <div class="section-title">
                    <h2 id="story-heading">داستان نگین</h2>
                </div>
                <div class="about-content">
                    <div class="about-text">
                        <p>
                            نگین از یک آرزوی ساده آغاز شد؛ آرزوی ایجاد خانه‌ای برای کودکانی که سال‌ها با کمبود فرصت‌های آموزشی و توان‌بخشی روبه‌رو بوده‌اند.
                        </p>
                        <p>
                            اسدالله حیدری و ساحل حیدری پس از سال‌ها مشاهدهٔ مشکلات و محرومیت‌های کودکان دارای معلولیت، تصمیم گرفتند این آرزو را به یک کار عملی تبدیل کنند.
                        </p>
                        <p>
                            در این مسیر، اجمیر خان میرزاد با حمایت و همراهی ارزشمند خود در کنار آنان قرار گرفت و به تحقق این برنامه کمک کرد.
                        </p>
                        <p>
                            امروز نگین تلاش می‌کند این راه را با تکیه بر دانش، انسانیت، همکاری خانواده‌ها و حمایت جامعه ادامه دهد.
                        </p>
                    </div>
                    <div>
                        <img src="https://images.unsplash.com/photo-1544717297-fa95b6ee9643?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" 
                             alt="کودکان در حال یادگیری" 
                             class="about-image" 
                             loading="lazy">
                    </div>
                </div>
            </section>

            <!-- FOUNDERS MESSAGE -->
            <section class="section" aria-labelledby="founders-heading">
                <div class="section-title">
                    <h2 id="founders-heading">پیام بنیان‌گذاران</h2>
                </div>
                <div class="about-content">
                    <div class="about-text">
                        <blockquote>
                            «سال‌ها پیش، وقتی به چشم‌های پرامید کودکان دارای معلولیت نگاه می‌کردیم، با خود عهد کردیم روزی محیطی بسازیم که در آن هیچ کودکی به خاطر تفاوت‌هایش کنار گذاشته نشود. امروز نگین آغاز تحقق آن آرزو است.»
                        </blockquote>
                        <p style="margin-top: var(--spacing-lg);">
                            <strong>اسدالله حیدری و ساحل حیدری</strong><br>
                            بنیان‌گذاران مرکز آموزشی و توان‌بخشی نگین
                        </p>
                        
                        <div style="margin-top: var(--spacing-xl); padding: var(--spacing-lg); background: var(--surface-soft); border-radius: var(--radius-lg);">
                            <p>
                                <strong>اجمیر خان میرزاد</strong><br>
                                مشاور ارشد و حامی کلیدی مرکز
                            </p>
                            <p style="margin-top: var(--spacing-md);">
                                «با اراده می‌توان، با همت می‌سازیم.»
                            </p>
                            <p style="margin-top: var(--spacing-md); font-style: italic;">
                                اجمیر خان میرزاد از همراهان کلیدی در مسیر شکل‌گیری مرکز نگین است. حمایت، مشوره و همراهی او در تبدیل یک آرزوی دیرینه به یک برنامهٔ عملی نقش مهمی داشته است.
                            </p>
                            <p style="margin-top: var(--spacing-md);">
                                برای نگین، ارزش این همراهی تنها در حمایت مادی خلاصه نمی‌شود؛ بلکه در باور به توانایی کودکان، مسئولیت اجتماعی و ایستادن در کنار یک هدف انسانی معنا پیدا می‌کند.
                            </p>
                            <p style="margin-top: var(--spacing-md);">
                                «این مرکز فقط یک ساختمان نیست؛ پاسخی به سال‌ها بی‌پاسخی است. من به این راه افتخار می‌کنم و از همه دعوت می‌کنم که در این مسیر انسانی همراه ما باشند.»
                            </p>
                            <p style="margin-top: var(--spacing-md);">
                                نگین از این همراهی سپاسگزار است و امیدوار است با همکاری افراد نیکوکار و مسئولیت‌پذیر، فرصت‌های بیشتری برای کودکان فراهم شود.
                            </p>
                        </div>
                    </div>
                    <div>
                        <img src="https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" 
                             alt="اجمیر خان میرزاد" 
                             class="about-image" 
                             loading="lazy">
                    </div>
                </div>
            </section>

            <!-- VISION, MISSION, VALUES -->
            <section class="section" aria-labelledby="vision-heading">
                <div class="section-title">
                    <h2 id="vision-heading">چشم‌انداز، مأموریت و ارزش‌های ما</h2>
                </div>
                
                <div class="cards-grid">
                    <div class="card">
                        <div class="card-icon">🌱</div>
                        <h3>چشم‌انداز</h3>
                        <p>
                            ایجاد جامعه‌ای فراگیر که در آن کودکان دارای معلولیت و نیازهای ویژه، بدون توجه به نوع یا شدت ناتوانی، به آموزش باکیفیت، خدمات توان‌بخشی و فرصت مشارکت اجتماعی دسترسی داشته باشند.
                        </p>
                    </div>
                    <div class="card">
                        <div class="card-icon">🎯</div>
                        <h3>مأموریت</h3>
                        <p>
                            ارائهٔ خدمات آموزشی، توان‌بخشی و حمایتی متناسب با نیازهای هر کودک و همکاری نزدیک با خانواده‌ها، به منظور تقویت توانایی‌ها، افزایش استقلال و بهبود کیفیت زندگی کودکان.
                        </p>
                    </div>
                </div>

                <div style="margin-top: var(--spacing-xl);">
                    <h3 style="color: var(--primary); margin-bottom: var(--spacing-lg);">❤️ ارزش‌های ما</h3>
                    <div class="disability-features">
                        <div class="feature-item">
                            <span class="feature-icon">❤️</span>
                            <span><strong>عشق و پذیرش:</strong> هر کودک با احترام و مهربانی پذیرفته می‌شود.</span>
                        </div>
                        <div class="feature-item">
                            <span class="feature-icon">💪</span>
                            <span><strong>باور به توانایی:</strong> ما به ظرفیت‌های کودکان باور داریم و برای رشد آن تلاش می‌کنیم.</span>
                        </div>
                        <div class="feature-item">
                            <span class="feature-icon">⚖️</span>
                            <span><strong>برابری:</strong> هر کودک حق آموزش، رشد و برخورداری از فرصت‌های برابر را دارد.</span>
                        </div>
                        <div class="feature-item">
                            <span class="feature-icon">🤝</span>
                            <span><strong>همکاری:</strong> خانواده، آموزگار، متخصص و جامعه در کنار هم می‌توانند تغییر پایدار ایجاد کنند.</span>
                        </div>
                        <div class="feature-item">
                            <span class="feature-icon">🤲</span>
                            <span><strong>مسئولیت‌پذیری:</strong> اعتماد خانواده‌ها و پشتیبانان برای ما یک مسئولیت ارزشمند است.</span>
                        </div>
                        <div class="feature-item">
                            <span class="feature-icon">💡</span>
                            <span><strong>نوآوری:</strong> از روش‌های نو و فناوری‌های مناسب برای بهبود آموزش و خدمات استفاده می‌کنیم.</span>
                        </div>
                    </div>
                </div>
            </section>

            <!-- MAIN ACTIVITIES -->
            <section class="section" aria-labelledby="activities-heading">
                <div class="section-title">
                    <h2 id="activities-heading">🧩 سه محور اصلی فعالیت</h2>
                </div>
                <div class="cards-grid">
                    <div class="card">
                        <div class="card-icon">📚</div>
                        <h3>آموزش تخصصی</h3>
                        <p>
                            برنامه‌های آموزشی متناسب با توانایی و نیاز هر کودک، با تمرکز بر رشد مهارت‌های آموزشی، شناختی، ارتباطی و اجتماعی.
                        </p>
                    </div>
                    <div class="card">
                        <div class="card-icon">🏥</div>
                        <h3>توان‌بخشی حرفه‌ای</h3>
                        <p>
                            ارائهٔ خدمات فیزیوتراپی، کاردرمانی، گفتاردرمانی و حمایت‌های روانی و اجتماعی توسط افراد متخصص، متناسب با نیاز کودک.
                        </p>
                    </div>
                    <div class="card">
                        <div class="card-icon">👨‍👩‍👧‍👦</div>
                        <h3>حمایت از خانواده</h3>
                        <p>
                            آگاهی‌دهی، مشوره و برنامه‌های آموزشی برای والدین؛ زیرا خانواده یکی از مهم‌ترین بخش‌های مسیر رشد کودک است.
                        </p>
                    </div>
                </div>
            </section>

            <!-- SERVICES -->
            <section id="services" class="section" aria-labelledby="services-heading" style="background: var(--surface-soft);">
                <div class="section-title">
                    <h2 id="services-heading">💎 خدمات نگین</h2>
                </div>
                <div class="services-grid">
                    <div class="service-card">
                        <div class="service-icon">📚</div>
                        <h3>آموزش ویژه</h3>
                    </div>
                    <div class="service-card">
                        <div class="service-icon">🗣️</div>
                        <h3>گفتاردرمانی</h3>
                    </div>
                    <div class="service-card">
                        <div class="service-icon">🤲</div>
                        <h3>کاردرمانی</h3>
                    </div>
                    <div class="service-card">
                        <div class="service-icon">🏃</div>
                        <h3>فیزیوتراپی</h3>
                    </div>
                    <div class="service-card">
                        <div class="service-icon">💬</div>
                        <h3>آموزش مهارت‌های ارتباطی</h3>
                    </div>
                    <div class="service-card">
                        <div class="service-icon">🖼️</div>
                        <h3>ارتباط تصویری</h3>
                    </div>
                    <div class="service-card">
                        <div class="service-icon">🔄</div>
                        <h3>ارتباط جایگزین و افزوده</h3>
                    </div>
                    <div class="service-card">
                        <div class="service-icon">👨‍👩‍👧</div>
                        <h3>حمایت و آموزش خانواده‌ها</h3>
                    </div>
                    <div class="service-card">
                        <div class="service-icon">🛠️</div>
                        <h3>وسایل و فناوری‌های کمکی</h3>
                    </div>
                    <div class="service-card">
                        <div class="service-icon">🤝</div>
                        <h3>حمایت اجتماعی</h3>
                    </div>
                </div>
            </section>

            <!-- SPECIALIZED SERVICES SECTION -->
            <section id="specialized-services" class="section" aria-labelledby="specialized-heading">
                <div class="section-title">
                    <h2 id="specialized-heading">🎯 خدمات تخصصی نگین</h2>
                    <p class="section-subtitle">آموزش، توانبخشی و حمایت تخصصی برای کودکان با نیازهای ویژه</p>
                </div>

                <div class="accordion-container">
                    <!-- آموزش ویژه -->
                    <div class="accordion-item">
                        <button class="accordion-header" aria-expanded="false" aria-controls="education-content">
                            <span class="accordion-icon">📚</span>
                            <span class="accordion-title">آموزش ویژه</span>
                            <span class="accordion-arrow">▼</span>
                        </button>
                        <div class="accordion-content" id="education-content" hidden>
                            <div class="accordion-body">
                                <p class="lead">
                                    در مرکز آموزشی و توان‌بخشی نگین باور داریم که هر کودک می‌تواند یاد بگیرد، رشد کند و مهارت‌های تازه به دست آورد؛
                                    اما مسیر یادگیری برای همه کودکان یکسان نیست.
                                </p>
                                
                                <h4>📖 آموزش ویژه چیست؟</h4>
                                <p>
                                    آموزش ویژه مجموعه‌ای از روش‌ها، برنامه‌ها و حمایت‌های آموزشی است که برای کودکانی طراحی می‌شود
                                    که برای یادگیری مؤثر، به روش آموزشی، محیط، زمان، ابزار یا حمایت اضافی نیاز دارند.
                                </p>
                                
                                <h4>🎯 اهداف آموزش ویژه</h4>
                                <div class="grid-2">
                                    <div>
                                        <h5>📚 اهداف آموزشی</h5>
                                        <ul>
                                            <li>شناخت حروف و اعداد</li>
                                            <li>تقویت خواندن و نوشتن</li>
                                            <li>تقویت مهارت‌های ریاضی</li>
                                            <li>افزایش تمرکز و توجه</li>
                                            <li>تقویت حافظه و مهارت‌های شناختی</li>
                                        </ul>
                                    </div>
                                    <div>
                                        <h5>🗣️ اهداف ارتباطی</h5>
                                        <ul>
                                            <li>تقویت ارتباط کلامی</li>
                                            <li>افزایش توانایی درک و بیان نیازها</li>
                                            <li>تقویت مهارت‌های شنیداری</li>
                                            <li>استفاده از روش‌های ارتباطی جایگزین</li>
                                        </ul>
                                    </div>
                                    <div>
                                        <h5>👥 اهداف اجتماعی</h5>
                                        <ul>
                                            <li>برقراری ارتباط با دیگران</li>
                                            <li>رعایت نوبت</li>
                                            <li>مشارکت در فعالیت‌های گروهی</li>
                                            <li>شناخت احساسات</li>
                                            <li>تقویت مهارت‌های همکاری</li>
                                        </ul>
                                    </div>
                                    <div>
                                        <h5>🧒 اهداف استقلال فردی</h5>
                                        <ul>
                                            <li>لباس پوشیدن</li>
                                            <li>غذا خوردن</li>
                                            <li>استفاده مناسب از وسایل شخصی</li>
                                            <li>رعایت بهداشت فردی</li>
                                            <li>انجام فعالیت‌های ساده روزمره</li>
                                        </ul>
                                    </div>
                                </div>
                                
                                <h4>👶 چه کودکانی می‌توانند بهره‌مند شوند؟</h4>
                                <div class="feature-cards">
                                    <div class="feature-card">
                                        <span class="feature-icon">🧩</span>
                                        <p>کودکان دارای معلولیت</p>
                                    </div>
                                    <div class="feature-card">
                                        <span class="feature-icon">🧠</span>
                                        <p>کودکان دارای نیازهای رشدی</p>
                                    </div>
                                    <div class="feature-card">
                                        <span class="feature-icon">📚</span>
                                        <p>کودکان دارای مشکلات یادگیری</p>
                                    </div>
                                    <div class="feature-card">
                                        <span class="feature-icon">🗣️</span>
                                        <p>کودکان دارای نیازهای ارتباطی</p>
                                    </div>
                                    <div class="feature-card">
                                        <span class="feature-icon">🌱</span>
                                        <p>کودکان نیازمند حمایت آموزشی فردی</p>
                                    </div>
                                </div>
                                
                                <h4>🎨 روش‌های آموزشی</h4>
                                <div class="method-grid">
                                    <div class="method-card">
                                        <span class="method-icon">👁️</span>
                                        <h5>آموزش دیداری</h5>
                                        <p>استفاده از تصاویر، کارت‌ها، اشیای واقعی</p>
                                    </div>
                                    <div class="method-card">
                                        <span class="method-icon">👂</span>
                                        <h5>آموزش شنیداری</h5>
                                        <p>توضیحات شفاهی، تکرار، آهنگ</p>
                                    </div>
                                    <div class="method-card">
                                        <span class="method-icon">✋</span>
                                        <h5>آموزش عملی</h5>
                                        <p>یادگیری از طریق انجام دادن</p>
                                    </div>
                                    <div class="method-card">
                                        <span class="method-icon">🎮</span>
                                        <h5>آموزش از طریق بازی</h5>
                                        <p>افزایش انگیزه و مشارکت</p>
                                    </div>
                                    <div class="method-card">
                                        <span class="method-icon">🔁</span>
                                        <h5>تکرار و تمرین</h5>
                                        <p>تقویت مهارت‌ها</p>
                                    </div>
                                    <div class="method-card">
                                        <span class="method-icon">🧩</span>
                                        <h5>آموزش گام‌به‌گام</h5>
                                        <p>تقسیم مهارت به مراحل کوچک</p>
                                    </div>
                                </div>
                                
                                <div class="info-box">
                                    <p><strong>💡 اصول ما:</strong></p>
                                    <ul>
                                        <li>احترام به کودک و حفظ کرامت انسانی</li>
                                        <li>فرصت برابر برای همه کودکان</li>
                                        <li>کودک‌محوری در برنامه‌ریزی</li>
                                        <li>همکاری با خانواده</li>
                                        <li>تمرکز بر پیشرفت فردی</li>
                                        <li>آموزش بدون تحقیر</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- کاردرمانی کودکان -->
                    <div class="accordion-item">
                        <button class="accordion-header" aria-expanded="false" aria-controls="occupational-content">
                            <span class="accordion-icon">🤲</span>
                            <span class="accordion-title">کاردرمانی کودکان</span>
                            <span class="accordion-arrow">▼</span>
                        </button>
                        <div class="accordion-content" id="occupational-content" hidden>
                            <div class="accordion-body">
                                <p class="lead">
                                    تقویت توانایی‌ها، افزایش استقلال و مشارکت کودک در فعالیت‌های روزمره
                                </p>
                                
                                <h4>🤲 کاردرمانی چیست؟</h4>
                                <p>
                                    کاردرمانی یک حرفه توانبخشی است که به افراد کمک می‌کند در فعالیت‌های مهم و روزمره زندگی
                                    مشارکت مؤثرتر داشته باشند. در کودکان، این فعالیت‌ها می‌توانند شامل بازی، یادگیری، نوشتن،
                                    لباس پوشیدن، غذا خوردن و فعالیت‌های اجتماعی باشند.
                                </p>
                                
                                <h4>🎯 اهداف کاردرمانی در نگین</h4>
                                <div class="grid-2">
                                    <div>
                                        <h5>🖐️ مهارت‌های حرکتی ظریف</h5>
                                        <p>کمک به کودک در استفاده بهتر از دست‌ها و انگشتان</p>
                                    </div>
                                    <div>
                                        <h5>🧠 مهارت‌های شناختی</h5>
                                        <p>حمایت از توجه، حافظه، برنامه‌ریزی و حل مسئله</p>
                                    </div>
                                    <div>
                                        <h5>👁️ هماهنگی چشم و دست</h5>
                                        <p>کمک به کودک برای هماهنگ‌کردن حرکات دست با اطلاعات دیداری</p>
                                    </div>
                                    <div>
                                        <h5>✏️ آمادگی برای نوشتن</h5>
                                        <p>تقویت مهارت‌های مورد نیاز برای گرفتن مداد و نوشتن</p>
                                    </div>
                                    <div>
                                        <h5>🧒 افزایش استقلال</h5>
                                        <p>کمک به کودک برای انجام فعالیت‌های شخصی و روزمره</p>
                                    </div>
                                    <div>
                                        <h5>🎮 تقویت مهارت‌های بازی</h5>
                                        <p>کمک به کودک برای مشارکت در بازی‌های فردی و گروهی</p>
                                    </div>
                                </div>
                                
                                <h4>👶 چه کودکانی به کاردرمانی نیاز دارند؟</h4>
                                <ul>
                                    <li>کودکان دارای مشکلات حرکتی</li>
                                    <li>کودکان دارای ضعف مهارت‌های حرکتی ظریف</li>
                                    <li>کودکان دارای مشکل در نوشتن یا استفاده از ابزارهای آموزشی</li>
                                    <li>کودکان دارای مشکل در فعالیت‌های روزمره</li>
                                    <li>کودکان دارای مشکل در هماهنگی حرکات</li>
                                    <li>کودکان دارای مشکل در پردازش حسی</li>
                                </ul>
                                
                                <h4>📊 ارزیابی اولیه کودک</h4>
                                <div class="assessment-grid">
                                    <div class="assessment-item">
                                        <span class="assessment-icon">🖐️</span>
                                        <p>مهارت‌های حرکتی ظریف</p>
                                    </div>
                                    <div class="assessment-item">
                                        <span class="assessment-icon">💪</span>
                                        <p>مهارت‌های حرکتی درشت</p>
                                    </div>
                                    <div class="assessment-item">
                                        <span class="assessment-icon">👁️</span>
                                        <p>هماهنگی چشم و دست</p>
                                    </div>
                                    <div class="assessment-item">
                                        <span class="assessment-icon">🧠</span>
                                        <p>مهارت‌های شناختی</p>
                                    </div>
                                    <div class="assessment-item">
                                        <span class="assessment-icon">✏️</span>
                                        <p>مهارت‌های پیش‌نوشتاری</p>
                                    </div>
                                    <div class="assessment-item">
                                        <span class="assessment-icon">👕</span>
                                        <p>مهارت‌های خودمراقبتی</p>
                                    </div>
                                    <div class="assessment-item">
                                        <span class="assessment-icon">🎨</span>
                                        <p>مشارکت در بازی</p>
                                    </div>
                                </div>
                                
                                <h4>🎨 فعالیت‌های کاردرمانی</h4>
                                <div class="activity-cards">
                                    <div class="activity-card">
                                        <span class="activity-icon">🧩</span>
                                        <p>جورکردن قطعات</p>
                                    </div>
                                    <div class="activity-card">
                                        <span class="activity-icon">🖍️</span>
                                        <p>رنگ‌آمیزی</p>
                                    </div>
                                    <div class="activity-card">
                                        <span class="activity-icon">✏️</span>
                                        <p>نقاشی</p>
                                    </div>
                                    <div class="activity-card">
                                        <span class="activity-icon">🔵</span>
                                        <p>گرفتن اشیای کوچک</p>
                                    </div>
                                    <div class="activity-card">
                                        <span class="activity-icon">🧱</span>
                                        <p>ساختن با قطعات</p>
                                    </div>
                                    <div class="activity-card">
                                        <span class="activity-icon">✂️</span>
                                        <p>فعالیت‌های مناسب با قیچی</p>
                                    </div>
                                </div>
                                
                                <div class="info-box">
                                    <p><strong>💡 هدف نهایی:</strong> کودک بتواند در حد توانایی خود بازی کند، یاد بگیرد، فعالیت‌های روزمره را انجام دهد، از توانایی‌های خود استفاده کند و استقلال بیشتری به دست آورد.</p>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- گفتاردرمانی کودکان -->
                    <div class="accordion-item">
                        <button class="accordion-header" aria-expanded="false" aria-controls="speech-content">
                            <span class="accordion-icon">🗣️</span>
                            <span class="accordion-title">گفتاردرمانی کودکان</span>
                            <span class="accordion-arrow">▼</span>
                        </button>
                        <div class="accordion-content" id="speech-content" hidden>
                            <div class="accordion-body">
                                <p class="lead">
                                    هر صدا، یک ارتباط؛ هر ارتباط، یک فرصت
                                </p>
                                
                                <h4>🗣️ گفتاردرمانی چیست؟</h4>
                                <p>
                                    گفتاردرمانی یکی از خدمات تخصصی توانبخشی است که می‌تواند بر زمینه‌هایی مانند گفتار، زبان،
                                    ارتباط، صداهای گفتاری، درک زبان، بیان زبان و مهارت‌های ارتباط اجتماعی تمرکز داشته باشد.
                                </p>
                                
                                <h4>🎯 اهداف گفتاردرمانی در نگین</h4>
                                <p>
                                    هدف اصلی، کمک به کودک برای ارتباط مؤثر و کاربردی است. برای هر کودک، اهداف متفاوتی می‌تواند تعیین شود:
                                </p>
                                <ul>
                                    <li>افزایش واژگان برای کودکی</li>
                                    <li>درک دستورهای ساده برای کودک دیگر</li>
                                    <li>استفاده از تصاویر یا روش ارتباطی جایگزین برای کودک دیگری</li>
                                </ul>
                                
                                <h4>👶 چه کودکانی به گفتاردرمانی نیاز دارند؟</h4>
                                <div class="grid-2">
                                    <div>
                                        <h5>🗣️ مشکلات گفتاری</h5>
                                        <p>دشواری در تولید یا تلفظ صداهای گفتاری</p>
                                    </div>
                                    <div>
                                        <h5>📚 مشکلات زبان</h5>
                                        <p>نیاز به حمایت در درک یا استفاده از زبان</p>
                                    </div>
                                    <div>
                                        <h5>💬 مشکلات ارتباطی</h5>
                                        <p>مشکل در بیان خواسته‌ها، نیازها و احساسات</p>
                                    </div>
                                    <div>
                                        <h5>🔊 مشکلات صدا</h5>
                                        <p>نیاز به ارزیابی کیفیت و شدت صدا</p>
                                    </div>
                                    <div>
                                        <h5>🔄 مشکلات روانی گفتار</h5>
                                        <p>دشواری در روان و جریان گفتار</p>
                                    </div>
                                    <div>
                                        <h5>🍽️ مشکلات تغذیه و بلع</h5>
                                        <p>ارزیابی تخصصی توسط متخصص مربوطه</p>
                                    </div>
                                </div>
                                
                                <h4>📊 ارزیابی گفتار و زبان</h4>
                                <div class="assessment-grid">
                                    <div class="assessment-item">
                                        <span class="assessment-icon">👂</span>
                                        <p>درک زبان</p>
                                    </div>
                                    <div class="assessment-item">
                                        <span class="assessment-icon">🗣️</span>
                                        <p>بیان زبان</p>
                                    </div>
                                    <div class="assessment-item">
                                        <span class="assessment-icon">🔤</span>
                                        <p>گفتار و تلفظ</p>
                                    </div>
                                    <div class="assessment-item">
                                        <span class="assessment-icon">💬</span>
                                        <p>مهارت‌های ارتباطی</p>
                                    </div>
                                    <div class="assessment-item">
                                        <span class="assessment-icon">👀</span>
                                        <p>ارتباط غیرکلامی</p>
                                    </div>
                                    <div class="assessment-item">
                                        <span class="assessment-icon">🧠</span>
                                        <p>مهارت‌های ارتباط اجتماعی</p>
                                    </div>
                                </div>
                                
                                <h4>🎨 روش‌های درمانی</h4>
                                <div class="method-grid">
                                    <div class="method-card">
                                        <span class="method-icon">🎲</span>
                                        <h5>بازی‌های نوبتی</h5>
                                    </div>
                                    <div class="method-card">
                                        <span class="method-icon">🧸</span>
                                        <h5>بازی‌های نقش‌آفرینی</h5>
                                    </div>
                                    <div class="method-card">
                                        <span class="method-icon">🧩</span>
                                        <h5>بازی‌های نام‌گذاری</h5>
                                    </div>
                                    <div class="method-card">
                                        <span class="method-icon">📚</span>
                                        <h5>داستان‌گویی</h5>
                                    </div>
                                    <div class="method-card">
                                        <span class="method-icon">🎵</span>
                                        <h5>فعالیت‌های آهنگین</h5>
                                    </div>
                                    <div class="method-card">
                                        <span class="method-icon">🖼️</span>
                                        <h5>بازی با تصاویر</h5>
                                    </div>
                                </div>
                                
                                <h4>💡 ارتباط جایگزین و تکمیلی</h4>
                                <p>
                                    برای برخی کودکان، استفاده از روش‌های ارتباط جایگزین و تکمیلی (AAC) مناسب است:
                                </p>
                                <div class="feature-cards">
                                    <div class="feature-card">
                                        <span class="feature-icon">🖼️</span>
                                        <p>تصاویر</p>
                                    </div>
                                    <div class="feature-card">
                                        <span class="feature-icon">👉</span>
                                        <p>اشاره</p>
                                    </div>
                                    <div class="feature-card">
                                        <span class="feature-icon">📋</span>
                                        <p>تخته‌های ارتباطی</p>
                                    </div>
                                    <div class="feature-card">
                                        <span class="feature-icon">📱</span>
                                        <p>ابزارهای دیجیتال</p>
                                    </div>
                                    <div class="feature-card">
                                        <span class="feature-icon">🔤</span>
                                        <p>نمادها و نشانه‌ها</p>
                                    </div>
                                </div>
                                
                                <div class="info-box">
                                    <p><strong>💡 اصول ما:</strong></p>
                                    <ul>
                                        <li>هر کودک مسیر متفاوتی دارد</li>
                                        <li>برنامه بر اساس نیازهای فردی تنظیم می‌شود</li>
                                        <li>ارتباط از طریق بازی طبیعی‌تر است</li>
                                        <li>همکاری خانواده بسیار مهم است</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- TEAM SECTION -->
            <section id="team" class="section" aria-labelledby="team-heading">
                <div class="section-title">
                    <h2 id="team-heading">👥 گروه کاری ما</h2>
                    <p class="section-subtitle">مرکز نگین با همکاری گروهی از افراد در بخش‌های گوناگون فعالیت می‌کند</p>
                </div>
                <div class="cards-grid">
                    <div class="card">
                        <div class="card-icon">👨</div>
                        <h3>اسدالله حیدری</h3>
                        <p><strong>بنیان‌گذار و مدیر اجرایی</strong></p>
                    </div>
                    <div class="card">
                        <div class="card-icon">👩</div>
                        <h3>ساحل حیدری</h3>
                        <p><strong>بنیان‌گذار و مدیر آموزشی</strong></p>
                    </div>
                    <div class="card">
                        <div class="card-icon">💼</div>
                        <h3>اجمیر خان میرزاد</h3>
                        <p><strong>مشاور ارشد و حامی کلیدی</strong></p>
                    </div>
                    <div class="card">
                        <div class="card-icon">👥</div>
                        <h3>گروه تخصصی</h3>
                        <p>آموزگاران آموزش ویژه، درمانگران، گفتاردرمان‌گران، کاردرمان‌گران، فیزیوتراپیست‌ها، روان‌شناسان و مددکاران اجتماعی، مطابق ظرفیت و نیاز مرکز</p>
                    </div>
                </div>
            </section>

            <!-- TECHNOLOGY SECTION -->
            <section class="section" aria-labelledby="tech-heading">
                <div class="section-title">
                    <h2 id="tech-heading">🧠 نگین و فناوری</h2>
                </div>
                <div class="about-content">
                    <div class="about-text">
                        <p>
                            نگین در کنار خدمات حضوری، به استفاده از فناوری برای آسان‌ترساختن آموزش و ارتباط نیز توجه دارد.
                        </p>
                        <p>
                            برنامه‌های آینده می‌تواند شامل ابزارهای ارتباطی، منابع آموزشی دیجیتالی، فناوری‌های کمکی و راهکارهای هوشمند برای کودکان، خانواده‌ها و آموزگاران باشد.
                        </p>
                        
                        <h3 style="margin-top: var(--spacing-lg);">نگین هوشمند</h3>
                        <p>
                            نگین هوشمند یک دستیار اطلاعاتی و آموزشی برای کمک به خانواده‌ها و آموزگاران در زمینهٔ آموزش ویژه، ارتباط و توان‌بخشی است.
                        </p>
                        <p>
                            این ابزار برای آگاهی‌دهی و دسترسی آسان‌تر به معلومات طراحی می‌شود و جایگزین تشخیص یا خدمات تخصصی درمانگران نیست.
                        </p>
                    </div>
                    <div>
                        <img src="https://images.unsplash.com/photo-1559757175-0eb30cd8c063?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" 
                             alt="فناوری در آموزش کودکان دارای معلولیت" 
                             class="about-image" 
                             loading="lazy">
                    </div>
                </div>
            </section>

            <!-- WHY NEGIN -->
            <section class="section" aria-labelledby="why-heading">
                <div class="section-title">
                    <h2 id="why-heading">❓ چرا نگین؟</h2>
                </div>
                <div class="about-content">
                    <div class="about-text">
                        <p>
                            بسیاری از کودکان دارای معلولیت با موانعی مانند کمبود فرصت‌های آموزشی، دسترسی محدود به خدمات توان‌بخشی، نبود ابزارهای مناسب و آگاهی ناکافی خانواده‌ها روبه‌رو هستند.
                        </p>
                        <p>
                            نگین تلاش می‌کند بخشی از این خلأ را با ایجاد یک محیط آموزشی، توان‌بخشی، خانواده‌محور و انسانی کاهش دهد.
                        </p>
                        <blockquote>
                            هدف ما این نیست که کودک را با محدودیتش تعریف کنیم؛ بلکه می‌خواهیم توانایی و ظرفیت او دیده شود.
                        </blockquote>
                    </div>
                    <div>
                        <img src="https://images.unsplash.com/photo-1594736797933-d0401ba2fe65?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" 
                             alt="کودک دارای معلولیت در حال یادگیری" 
                             class="about-image" 
                             loading="lazy">
                    </div>
                </div>
            </section>

            <!-- COLLABORATION -->
            <section class="section" aria-labelledby="collab-heading">
                <div class="section-title">
                    <h2 id="collab-heading">🤲 دعوت به همکاری</h2>
                    <p class="section-subtitle">برای گسترش خدمات و حمایت از کودکان بیشتر، همکاری جامعه ضروری است</p>
                </div>
                <div class="cards-grid">
                    <div class="card">
                        <div class="card-icon">💰</div>
                        <h3>پشتیبانی مالی</h3>
                        <p>برای توسعهٔ خدمات و حمایت از کودکان نیازمند</p>
                    </div>
                    <div class="card">
                        <div class="card-icon">🎁</div>
                        <h3>اهدای وسایل آموزشی و توان‌بخشی</h3>
                        <p>برای فراهم‌سازی امکانات مورد نیاز کودکان</p>
                    </div>
                    <div class="card">
                        <div class="card-icon">👩‍🏫</div>
                        <h3>همکاری تخصصی</h3>
                        <p>با آموزگاران، درمانگران و متخصصان</p>
                    </div>
                    <div class="card">
                        <div class="card-icon">🤝</div>
                        <h3>همکاری داوطلبانه</h3>
                        <p>با اختصاص زمان، مهارت و توانایی</p>
                    </div>
                    <div class="card">
                        <div class="card-icon">🏢</div>
                        <h3>همکاری سازمانی</h3>
                        <p>برای ایجاد برنامه‌های مشترک و پایدار</p>
                    </div>
                </div>
                <p style="text-align: center; margin-top: var(--spacing-lg); font-size: var(--font-size-lg); color: var(--primary);">
                    هر همکاری می‌تواند یک فرصت تازه برای یک کودک باشد
                </p>
            </section>

            <!-- MESSAGE TO FAMILIES -->
            <section class="section" aria-labelledby="families-heading">
                <div class="section-title">
                    <h2 id="families-heading">💙 سخن ما با خانواده‌ها</h2>
                </div>
                <div style="text-align: center; padding: var(--spacing-xl); background: var(--surface-soft); border-radius: var(--radius-xl);">
                    <p style="font-size: var(--font-size-lg); line-height: 2; color: var(--text);">
                        ممکن است هر کودک با سرعت و روش متفاوتی یاد بگیرد؛ اما همهٔ کودکان شایستهٔ احترام، آموزش و فرصت رشد هستند.
                    </p>
                    <p style="margin-top: var(--spacing-lg); font-size: var(--font-size-lg); color: var(--text);">
                        نگین می‌خواهد در کنار خانواده‌ها باشد تا کودکان بتوانند با حمایت مناسب، توانایی‌های خود را بهتر بشناسند و مسیر آیندهٔ خود را با امید بیشتری دنبال کنند.
                    </p>
                </div>
            </section>

            <!-- NEGIN MESSAGE -->
            <section class="section" aria-labelledby="message-heading">
                <div class="section-title">
                    <h2 id="message-heading">✨ پیام نگین</h2>
                </div>
                <div style="text-align: center; padding: var(--spacing-xl);">
                    <p style="font-size: var(--font-size-lg); line-height: 2; color: var(--text);">
                        ما باور داریم که آیندهٔ هر کودک تنها با محدودیت‌های امروز او تعیین نمی‌شود.
                    </p>
                    <p style="margin-top: var(--spacing-lg); font-size: var(--font-size-lg); color: var(--text);">
                        گاهی یک فرصت آموزشی، یک جلسهٔ توان‌بخشی، یک وسیلهٔ ارتباطی، یک آموزگار دلسوز، یا یک خانوادهٔ آگاه می‌تواند مسیر زندگی یک کودک را تغییر دهد.
                    </p>
                    <p style="margin-top: var(--spacing-lg); font-size: var(--font-size-xl); font-weight: 700; color: var(--primary);">
                        مرکز آموزشی و توان‌بخشی نگین<br>
                        جایی برای آموزش، توان‌بخشی، ارتباط و امید
                    </p>
                    <p style="margin-top: var(--spacing-md); font-size: var(--font-size-xl); color: var(--gold);">
                        💎 «هر کودک، یک نگین»
                    </p>
                </div>
            </section>

            <!-- EDUCATION SECTION (from user's code) -->
            <section id="education">
                <div class="hero" style="background: linear-gradient(135deg, var(--primary-dark), var(--primary)); color: white;">
                    <div class="hero-content">
                        <h2 style="color: white; font-size: 2.5rem; margin-bottom: var(--spacing-md);">📚 آموزش برای هر کودک</h2>
                        <p style="color: rgba(255,255,255,0.9);">
                            در مرکز آموزشی و توان‌بخشی نگین، آموزش را به شیوه‌ای آسان، جذاب، تعاملی و دسترس‌پذیر برای کودکان فراهم می‌کنیم.
                        </p>
                        <div class="cta-buttons">
                            <a href="#games" class="btn" style="background: var(--gold); color: #111;">🎮 شروع بازی آموزشی</a>
                            <a href="#library" class="btn" style="background: white; color: var(--primary-dark);">📚 ورود به کتابخانه</a>
                        </div>
                    </div>
                </div>

                <div class="section">
                    <div class="section-title">
                        <h2>یادگیری آسان و جذاب</h2>
                        <p>کودک می‌تواند با بازی، تصویر، صدا و ویدیو یاد بگیرد.</p>
                    </div>
                    <div class="cards-grid">
                        <div class="card">
                            <div class="card-icon">🎮</div>
                            <h3>بازی‌های آموزشی</h3>
                            <p>بازی‌های ساده و تعاملی برای تقویت یادگیری و مهارت‌های کودک.</p>
                            <a href="#games">مشاهده بازی‌ها ←</a>
                        </div>
                        <div class="card">
                            <div class="card-icon">🎬</div>
                            <h3>ویدیوهای آموزشی</h3>
                            <p>ویدیوهای آموزشی با امکان استفاده از زیرنویس و زبان اشاره.</p>
                            <a href="#videos">مشاهده ویدیوها ←</a>
                        </div>
                        <div class="card">
                            <div class="card-icon">📚</div>
                            <h3>کتابخانه دیجیتال</h3>
                            <p>دسترسی به کتاب‌های تصویری، صوتی و محتوای آموزشی.</p>
                            <a href="#library">ورود به کتابخانه ←</a>
                        </div>
                        <div class="card">
                            <div class="card-icon">👨‍👩‍👧</div>
                            <h3>راهنمای والدین</h3>
                            <p>مقالات و راهنماهای کاربردی برای خانواده‌ها.</p>
                            <a href="#parents">راهنمای والدین ←</a>
                        </div>
                    </div>
                </div>

                <!-- GAME SECTION -->
                <section id="games" class="section">
                    <div class="section-title">
                        <h2>🎮 بازی‌های آموزشی تعاملی</h2>
                        <p>یک بازی ساده برای تمرین شناخت اعداد</p>
                    </div>
                    <div class="card game-card">
                        <h3>عدد درست را انتخاب کنید</h3>
                        <div class="game-box">
                            <div class="game-question" id="gameQuestion">عدد ۳ را پیدا کنید</div>
                            <div class="game-options">
                                <button onclick="checkAnswer(1)">1</button>
                                <button onclick="checkAnswer(3)">3</button>
                                <button onclick="checkAnswer(5)">5</button>
                                <button onclick="checkAnswer(7)">7</button>
                            </div>
                            <div id="gameMessage" class="game-message" aria-live="polite"></div>
                        </div>
                    </div>
                </section>

                <!-- VIDEO SECTION -->
                <section id="videos" class="section">
                    <div class="section-title">
                        <h2>🎬 ویدیوهای آموزشی</h2>
                        <p>محتوای آموزشی مناسب کودکان با نیازهای گوناگون</p>
                    </div>
                    <div class="cards-grid">
                        <div class="card video-card">
                            <div class="video-placeholder">▶</div>
                            <h3>آشنایی با رنگ‌ها</h3>
                            <p>آموزش رنگ‌ها با تصویر و صدا.</p>
                            <div class="video-controls">
                                <button onclick="showToast('زیرنویس فعال شد')">📝 زیرنویس</button>
                                <button onclick="showToast('بخش زبان اشاره فعال شد')">🤟 زبان اشاره</button>
                                <button onclick="showToast('پخش ویدیو آغاز شد')">▶ پخش</button>
                            </div>
                        </div>
                        <div class="card video-card">
                            <div class="video-placeholder">▶</div>
                            <h3>آموزش اعداد</h3>
                            <p>یادگیری اعداد به شکل تصویری و سرگرم‌کننده.</p>
                            <div class="video-controls">
                                <button onclick="showToast('زیرنویس فعال شد')">📝 زیرنویس</button>
                                <button onclick="showToast('زبان اشاره فعال شد')">🤟 زبان اشاره</button>
                                <button onclick="showToast('پخش ویدیو آغاز شد')">▶ پخش</button>
                            </div>
                        </div>
                        <div class="card video-card">
                            <div class="video-placeholder">▶</div>
                            <h3>مهارت‌های روزمره</h3>
                            <p>آموزش مهارت‌های ساده و کاربردی زندگی روزمره.</p>
                            <div class="video-controls">
                                <button onclick="showToast('زیرنویس فعال شد')">📝 زیرنویس</button>
                                <button onclick="showToast('زبان اشاره فعال شد')">🤟 زبان اشاره</button>
                                <button onclick="showToast('پخش ویدیو آغاز شد')">▶ پخش</button>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- LIBRARY SECTION -->
                <section id="library" class="section">
                    <div class="section-title">
                        <h2>📚 کتابخانه دیجیتال</h2>
                        <p>کتاب‌های تصویری و صوتی برای یادگیری و سرگرمی</p>
                    </div>
                    <div class="library-filter">
                        <button class="active" onclick="filterLibrary('all',this)">همه</button>
                        <button onclick="filterLibrary('audio',this)">🔊 صوتی</button>
                        <button onclick="filterLibrary('picture',this)">🖼️ تصویری</button>
                    </div>
                    <div class="cards-grid" id="libraryCards">
                        <div class="card library-item" data-type="picture">
                            <div class="card-icon">🖼️</div>
                            <h3>داستان کودکانه</h3>
                            <p>یک داستان تصویری برای تقویت تخیل کودک.</p>
                            <button onclick="showToast('کتاب تصویری باز شد')">📖 مطالعه</button>
                        </div>
                        <div class="card library-item" data-type="audio">
                            <div class="card-icon">🔊</div>
                            <h3>داستان صوتی</h3>
                            <p>داستان کوتاه با صدای قابل فهم برای کودکان.</p>
                            <button onclick="showToast('پخش کتاب صوتی آغاز شد')">▶ پخش صوت</button>
                        </div>
                        <div class="card library-item" data-type="picture">
                            <div class="card-icon">🌈</div>
                            <h3>رنگ‌های شاد</h3>
                            <p>کتاب تصویری آموزش رنگ‌ها.</p>
                            <button onclick="showToast('کتاب باز شد')">📖 مطالعه</button>
                        </div>
                        <div class="card library-item" data-type="audio">
                            <div class="card-icon">🎧</div>
                            <h3>آموزش اعداد</h3>
                            <p>محتوای صوتی برای یادگیری اعداد.</p>
                            <button onclick="showToast('فایل صوتی پخش شد')">▶ پخش صوت</button>
                        </div>
                    </div>
                </section>

                <!-- PARENTS SECTION -->
                <section id="parents" class="section">
                    <div class="section-title">
                        <h2>👨‍👩‍👧 مقالات و راهنماهای والدین</h2>
                        <p>اطلاعات کاربردی برای حمایت بهتر از رشد و یادگیری کودک</p>
                    </div>
                    <div class="cards-grid">
                        <div class="card guide">
                            <h3>چگونه به کودک در یادگیری کمک کنیم؟</h3>
                            <p>راهکارهای ساده برای ایجاد محیط مناسب یادگیری در خانه.</p>
                            <button onclick="showToast('راهنما باز شد')">مطالعه راهنما</button>
                        </div>
                        <div class="card guide">
                            <h3>اهمیت بازی در رشد کودک</h3>
                            <p>چگونه بازی می‌تواند مهارت‌های شناختی و اجتماعی کودک را تقویت کند؟</p>
                            <button onclick="showToast('مقاله باز شد')">مطالعه مقاله</button>
                        </div>
                        <div class="card guide">
                            <h3>حمایت از کودک با نیازهای ویژه</h3>
                            <p>راهنمای خانواده برای ایجاد محیطی امن، حمایتگر و مناسب.</p>
                            <button onclick="showToast('راهنما باز شد')">مطالعه راهنما</button>
                        </div>
                    </div>
                </section>
            </section>

            <!-- CONTACT SECTION -->
            <section id="contact" class="section" aria-labelledby="contact-heading">
                <div class="section-title">
                    <h2 id="contact-heading">📞 اطلاعات تماس</h2>
                </div>
                <div class="about-content">
                    <div class="about-text">
                        <h3>مرکز آموزشی و توان‌بخشی نگین</h3>
                        <p><strong>مؤسسه‌ی خدماتی و حرفه‌ای زنان بی‌بضاعت</strong></p>
                        
                        <div style="margin-top: var(--spacing-lg);">
                            <p><strong>📍 نشانی:</strong></p>
                            <p>کابل، پروژهٔ وزیرآباد، سرک ۳۷، افغانستان</p>
                            
                            <p style="margin-top: var(--spacing-md);"><strong>📞 شمارهٔ تماس:</strong></p>
                            <p>۰۷۸۶۸۳۸۰۰۲</p>
                            
                            <p style="margin-top: var(--spacing-md);"><strong>📧 نشانی برقی:</strong></p>
                            <p><a href="mailto:negineducationcenter@gmail.com" style="color: var(--primary);">negineducationcenter@gmail.com</a></p>
                            
                            <p style="margin-top: var(--spacing-md);"><strong>🕐 ساعات کاری:</strong></p>
                            <p>شنبه تا چهارشنبه: ۸ صبح تا ۴ بعدازظهر</p>
                            <p>پنجشنبه: ۸ صبح تا ۱۲ ظهر</p>
                            
                            <p style="margin-top: var(--spacing-md);"><strong>📍 موقعیت مرکز در نقشه:</strong></p>
                            <p><a href="https://maps.app.goo.gl/UTwdrbUfqR6ewS9D9" target="_blank" style="color: var(--primary);">مشاهده در گوگل مپ</a></p>
                        </div>
                        
                        <p style="margin-top: var(--spacing-xl); font-size: var(--font-size-xl); color: var(--primary);">
                            مرکز آموزشی و توان‌بخشی نگین<br>
                            «هر کودک، یک نگین» 💎
                        </p>
                        <p style="margin-top: var(--spacing-md); font-size: var(--font-size-lg); color: var(--gold-dark);">
                            با اراده می‌توان، با همت می‌سازیم.
                        </p>
                    </div>
                    <div>
                        <img src="https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" 
                             alt="مرکز آموزشی و توان‌بخشی نگین" 
                             class="about-image" 
                             loading="lazy">
                    </div>
                </div>

                <!-- NEGIN CONTACT FORM -->
                <div style="margin-top: var(--spacing-xl);">
                    <section id="contact-form" class="negin-contact-section">
                        <div class="negin-contact-header">
                            <span class="negin-contact-badge">📩 ارتباط با نگین</span>
                            <h2>با مرکز آموزشی و توان‌بخشی نگین در تماس باشید</h2>
                            <p>برای ثبت درخواست، دریافت اطلاعات، همکاری، داوطلبی، حمایت از کودکان یا پرسش درباره خدمات مرکز، فرم زیر را تکمیل کنید.</p>
                        </div>
                        <form class="negin-contact-form" action="https://formsubmit.co/negineducationcenter@gmail.com" method="POST">
                            <input type="hidden" name="_subject" value="پیام جدید از وبسایت مرکز آموزشی و توان‌بخشی نگین">
                            <input type="hidden" name="_template" value="table">
                            <input type="hidden" name="_captcha" value="true">
                            <input type="hidden" name="_next" value="https://naginagaidari.github.io/negin-education.github.io/">
                            <div class="negin-form-grid">
                                <div class="negin-form-group">
                                    <label for="name">نام و نام خانوادگی <span>*</span></label>
                                    <input type="text" id="name" name="نام و نام خانوادگی" placeholder="نام و نام خانوادگی خود را وارد کنید" required autocomplete="name">
                                </div>
                                <div class="negin-form-group">
                                    <label for="phone">شماره تماس <span>*</span></label>
                                    <input type="tel" id="phone" name="شماره تماس" placeholder="مثلاً ۰۷۸۶۸۳۸۰۰۲" required autocomplete="tel">
                                </div>
                                <div class="negin-form-group">
                                    <label for="email">ایمیل</label>
                                    <input type="email" id="email" name="ایمیل فرستنده" placeholder="example@gmail.com" autocomplete="email">
                                </div>
                                <div class="negin-form-group">
                                    <label for="request">موضوع درخواست <span>*</span></label>
                                    <select id="request" name="موضوع درخواست" required>
                                        <option value="">موضوع را انتخاب کنید</option>
                                        <option value="ثبت نام کودک">🧒 ثبت‌نام کودک</option>
                                        <option value="درخواست خدمات توانبخشی">♿ درخواست خدمات توانبخشی</option>
                                        <option value="آموزش ویژه">📚 آموزش ویژه</option>
                                        <option value="فیزیوتراپی">🏃 فیزیوتراپی</option>
                                        <option value="کاردرمانی">🤲 کاردرمانی</option>
                                        <option value="گفتاردرمانی">🗣️ گفتاردرمانی</option>
                                        <option value="روانشناسی و مشاوره">🧠 روان‌شناسی و مشاوره</option>
                                        <option value="کمک مالی">💛 کمک مالی</option>
                                        <option value="داوطلبی">🤝 داوطلبی</option>
                                        <option value="همکاری سازمانی">🏢 همکاری سازمانی</option>
                                        <option value="سایر">💬 سایر</option>
                                    </select>
                                </div>
                                <div class="negin-form-group">
                                    <label for="child-name">نام کودک</label>
                                    <input type="text" id="child-name" name="نام کودک" placeholder="در صورت نیاز">
                                </div>
                                <div class="negin-form-group">
                                    <label for="child-age">سن کودک</label>
                                    <input type="number" id="child-age" name="سن کودک" min="1" max="30" placeholder="سن کودک">
                                </div>
                            </div>
                            <div class="negin-form-group">
                                <label for="disability">نوع نیاز یا معلولیت</label>
                                <select id="disability" name="نوع نیاز یا معلولیت">
                                    <option value="">انتخاب کنید</option>
                                    <option value="اوتیسم">🧩 اوتیسم</option>
                                    <option value="ADHD">⚡ ADHD</option>
                                    <option value="معلولیت حرکتی">♿ معلولیت حرکتی</option>
                                    <option value="معلولیت بینایی">👁️ معلولیت بینایی</option>
                                    <option value="معلولیت شنوایی">👂 معلولیت شنوایی</option>
                                    <option value="اختلال گفتار و زبان">🗣️ گفتار و زبان</option>
                                    <option value="ناتوانی یادگیری">📖 ناتوانی یادگیری</option>
                                    <option value="کم‌توانی ذهنی">🧠 کم‌توانی ذهنی</option>
                                    <option value="چندمعلولیتی">🔗 چندمعلولیتی</option>
                                    <option value="سایر">سایر</option>
                                </select>
                            </div>
                            <div class="negin-form-group">
                                <label for="message">پیام شما <span>*</span></label>
                                <textarea id="message" name="پیام" rows="7" placeholder="پیام، پرسش یا درخواست خود را اینجا بنویسید..." required></textarea>
                            </div>
                            <label class="negin-consent">
                                <input type="checkbox" name="رضایت" value="با ارسال این فرم، با ارسال اطلاعات برای مرکز موافقم." required>
                                <span>با ارسال این فرم، با استفاده از اطلاعات واردشده برای پاسخ‌گویی به درخواست من موافقم.</span>
                            </label>
                            <button type="submit" class="negin-submit"><span>📨</span> ارسال درخواست</button>
                            <p class="negin-email-note">📧 پیام شما مستقیماً به ایمیل مرکز ارسال می‌شود: <strong>negineducationcenter@gmail.com</strong></p>
                        </form>
                    </section>
                </div>
            </section>
        </main>
    </div>

    <!-- =====================================================
         FOOTER
    ===================================================== -->
    <footer>
        <div class="footer-container">
            <div class="footer-grid">
                <div>
                    <h3>مرکز آموزشی و توان‌بخشی نگین</h3>
                    <p>مؤسسه‌ی خدماتی و حرفه‌ای زنان بی‌بضاعت</p>
                    <p>«هر کودک، یک نگین» 💎</p>
                </div>
                <div>
                    <h3>لینک‌های سریع</h3>
                    <ul>
                        <li><a href="#home">صفحه اصلی</a></li>
                        <li><a href="#about">درباره ما</a></li>
                        <li><a href="#story">داستان نگین</a></li>
                        <li><a href="#services">خدمات</a></li>
                        <li><a href="#education">آموزش</a></li>
                        <li><a href="#games">بازی‌ها</a></li>
                        <li><a href="#videos">ویدیوها</a></li>
                        <li><a href="#library">کتابخانه</a></li>
                        <li><a href="#parents">راهنمای والدین</a></li>
                        <li><a href="#contact">تماس با ما</a></li>
                    </ul>
                </div>
                <div>
                    <h3>تماس با ما</h3>
                    <ul>
                        <li>📍 کابل، پروژهٔ وزیرآباد، سرک ۳۷</li>
                        <li>📞 ۰۷۸۶۸۳۸۰۰۲</li>
                        <li>📧 negineducationcenter@gmail.com</li>
                    </ul>
                </div>
                <div>
                    <h3>دسترسی</h3>
                    <ul>
                        <li><a href="#">♿ امکانات دسترس‌پذیری</a></li>
                        <li><a href="https://maps.app.goo.gl/UTwdrbUfqR6ewS9D9" target="_blank">🗺️ نقشه گوگل</a></li>
                    </ul>
                </div>
            </div>
            <div class="footer-bottom">
                <p>© ۱۴۰۵ مرکز آموزشی و توان‌بخشی نگین | «هر کودک، یک نگین» 💎</p>
                <p style="margin-top: var(--spacing-xs);">با اراده می‌توان، با همت می‌سازیم.</p>
            </div>
        </div>
    </footer>

    <!-- =====================================================
         CHATBOT
    ===================================================== -->
    <div class="chatbot-container">
        <button class="chatbot-toggle" id="chatbotToggle" aria-label="باز کردن چت‌بات">💬</button>
        <div class="chatbot-popup" id="chatbotPopup">
            <div class="chatbot-header">
                <h4>چت‌بات نگین</h4>
                <button class="chatbot-close" id="chatbotClose" aria-label="بستن چت‌بات">×</button>
            </div>
            <div class="chatbot-messages" id="chatbotMessages">
                <div class="chatbot-message bot">
                    سلام! به چت‌بات مرکز آموزشی و توان‌بخشی نگین خوش آمدید. 💎
                </div>
                <div class="chatbot-message bot">
                    من اینجا هستم تا به سوالات شما درباره معلولیت، خدمات ما و مرکز نگین پاسخ دهم.
                </div>
            </div>
            <div class="chatbot-input-container">
                <input type="text" class="chatbot-input" id="chatbotInput" placeholder="سوال خود را تایپ کنید..." aria-label="ورودی چت‌بات">
                <button class="chatbot-send" id="chatbotSend" aria-label="ارسال پیام">ارسال</button>
            </div>
        </div>
    </div>

    <!-- =====================================================
         SIDEBAR TOGGLE BUTTON
    ===================================================== -->
    <button class="sidebar-toggle" id="sidebarToggle" aria-label="نمایش/مخفی کردن منوی جانبی" aria-expanded="false" aria-controls="sidebar">
        منوی جانبی ☰
    </button>

    <!-- =====================================================
         TOAST NOTIFICATION
    ===================================================== -->
    <div id="toast" class="toast" role="status" aria-live="polite"></div>

    <script>
        // =====================================================
        // IMAGE SLIDER
        // =====================================================
        let currentSlide = 0;
        const slides = document.querySelectorAll('.slide');
        const dotsContainer = document.getElementById('sliderDots');
        
        function createDots() {
            slides.forEach((_, index) => {
                const dot = document.createElement('button');
                dot.classList.add('dot');
                if (index === 0) dot.classList.add('active');
                dot.onclick = () => goToSlide(index);
                dot.ariaLabel = `برو به اسلاید ${index + 1}`;
                dotsContainer.appendChild(dot);
            });
        }

        function goToSlide(index) {
            currentSlide = index;
            const slider = document.getElementById('imageSlider');
            slider.style.transform = `translateX(-${currentSlide * 100}%)`;
            updateDots();
        }

        function updateDots() {
            const dots = document.querySelectorAll('.dot');
            dots.forEach((dot, index) => {
                dot.classList.toggle('active', index === currentSlide);
            });
        }

        function nextSlide() {
            currentSlide = (currentSlide + 1) % slides.length;
            goToSlide(currentSlide);
        }

        // Initialize slider
        createDots();
        setInterval(nextSlide, 5000); // Change slide every 5 seconds

        // =====================================================
        // MOBILE MENU TOGGLE
        // =====================================================
        document.addEventListener('DOMContentLoaded', function() {
            const mobileMenuBtn = document.querySelector('.mobile-menu-btn');
            const navLinks = document.getElementById('nav-links');
            
            if (mobileMenuBtn && navLinks) {
                mobileMenuBtn.addEventListener('click', function() {
                    const isExpanded = this.getAttribute('aria-expanded') === 'true';
                    this.setAttribute('aria-expanded', !isExpanded);
                    navLinks.classList.toggle('active');
                });
            }

            // =====================================================
            // SIDEBAR DISABILITY TYPES TOGGLE
            // =====================================================
            const disabilityTypes = document.querySelectorAll('.disability-type');
            const disabilityContents = document.querySelectorAll('.disability-content');
            
            disabilityTypes.forEach(type => {
                type.addEventListener('click', function() {
                    const target = this.getAttribute('data-target');
                    
                    disabilityTypes.forEach(t => t.classList.remove('active'));
                    this.classList.add('active');
                    
                    disabilityContents.forEach(content => {
                        content.classList.remove('active');
                    });
                    
                    const targetContent = document.getElementById(target);
                    if (targetContent) {
                        targetContent.classList.add('active');
                        document.getElementById('main-content').scrollIntoView({
                            behavior: 'smooth',
                            block: 'start'
                        });
                    }
                });
            });

            // =====================================================
            // SIDEBAR TOGGLE FOR MOBILE/TABLET
            // =====================================================
            const sidebarToggle = document.getElementById('sidebarToggle');
            const sidebar = document.getElementById('sidebar');
            
            if (sidebarToggle && sidebar) {
                sidebarToggle.addEventListener('click', function() {
                    const isExpanded = this.getAttribute('aria-expanded') === 'true';
                    this.setAttribute('aria-expanded', !isExpanded);
                    sidebar.classList.toggle('active');
                });
            }

            // =====================================================
            // ACCESSIBILITY CONTROLS
            // =====================================================
            let fontSize = 100;

            window.increaseText = function() {
                fontSize += 10;
                if (fontSize > 160) fontSize = 160;
                document.documentElement.style.fontSize = fontSize + '%';
                localStorage.setItem('fontSize', fontSize);
            };

            window.decreaseText = function() {
                fontSize -= 10;
                if (fontSize < 80) fontSize = 80;
                document.documentElement.style.fontSize = fontSize + '%';
                localStorage.setItem('fontSize', fontSize);
            };

            window.resetText = function() {
                fontSize = 100;
                document.documentElement.style.fontSize = '100%';
                localStorage.setItem('fontSize', 100);
            };

            window.toggleDark = function() {
                document.body.classList.toggle('dark');
                localStorage.setItem('darkMode', document.body.classList.contains('dark'));
            };

            window.toggleContrast = function() {
                document.body.classList.toggle('high-contrast');
                localStorage.setItem('highContrast', document.body.classList.contains('high-contrast'));
            };

            // Load saved preferences
            if (localStorage.getItem('fontSize')) {
                fontSize = parseInt(localStorage.getItem('fontSize'));
                document.documentElement.style.fontSize = fontSize + '%';
            }
            if (localStorage.getItem('darkMode') === 'true') {
                document.body.classList.add('dark');
            }
            if (localStorage.getItem('highContrast') === 'true') {
                document.body.classList.add('high-contrast');
            }

            // =====================================================
            // ACCORDION FUNCTIONALITY
            // =====================================================
            document.querySelectorAll('.accordion-header').forEach(header => {
                header.addEventListener('click', () => {
                    const item = header.parentElement;
                    const isExpanded = item.getAttribute('aria-expanded') === 'true';
                    
                    // Close all other accordions
                    document.querySelectorAll('.accordion-item').forEach(otherItem => {
                        if (otherItem !== item) {
                            otherItem.setAttribute('aria-expanded', 'false');
                            otherItem.querySelector('.accordion-content').hidden = true;
                        }
                    });
                    
                    // Toggle current accordion
                    item.setAttribute('aria-expanded', !isExpanded);
                    header.nextElementSibling.hidden = isExpanded;
                });
            });

            // =====================================================
            // CHATBOT
            // =====================================================
            const chatbotToggle = document.getElementById('chatbotToggle');
            const chatbotPopup = document.getElementById('chatbotPopup');
            const chatbotClose = document.getElementById('chatbotClose');
            const chatbotInput = document.getElementById('chatbotInput');
            const chatbotSend = document.getElementById('chatbotSend');
            const chatbotMessages = document.getElementById('chatbotMessages');

            // Chatbot knowledge base
            const chatbotKnowledge = {
                "سلام": ["سلام! 💎 به چت‌بات مرکز آموزشی و توان‌بخشی نگین خوش آمدید.", "چطور میتونم کمکتون کنم؟"],
                "چطوری": ["عالی هستم، ممنون. شما چطورید؟"],
                "شما کی هستید": ["من چت‌بات مرکز آموزشی و توان‌بخشی نگین هستم. اینجا هستم تا به سوالات شما درباره معلولیت و خدمات ما پاسخ دهم."],
                "نگین چیست": [
                    "مرکز آموزشی و توان‌بخشی نگین یک مرکز تخصصی برای آموزش، توان‌بخشی و حمایت از کودکان دارای معلولیت و نیازهای آموزشی ویژه است.",
                    "ما در کابل، افغانستان فعالیت می‌کنیم."
                ],
                "مؤسسه نگین": [
                    "مرکز آموزشی و توان‌بخشی نگین تحت نظر مؤسسه‌ی خدماتی و حرفه‌ای زنان بی‌بضاعت فعالیت می‌کند.",
                    "هدف ما ایجاد محیطی امن برای رشد و شکوفایی کودکان دارای معلولیت است."
                ],
                "هر کودک یک نگین": ["بله! شعار ما «هر کودک، یک نگین» 💎 است. ما باور داریم هر کودک با ارزش و منحصر به فرد است."],
                "انواع معلولیت": [
                    "انواع معلولیت شامل: جسمی و حرکتی، بینایی، شنوایی، مشکلات گفتاری و ارتباطی، مشکلات یادگیری، اختلالات رشدی، معلولیت‌های چندگانه و نیازهای حمایتی ویژه می‌شود.",
                    "هر کدام از این معلولیت‌ها ویژگی‌ها و چالش‌های خاص خود را دارند."
                ],
                "معلولیت جسمی": [
                    "معلولیت جسمی و حرکتی به محدودیت‌های جسمانی اشاره دارد که بر توانایی حرکت و هماهنگی تأثیر می‌گذارد.",
                    "انواع آن شامل فلج مغزی، ضایعات نخاعی، آمپوتاسیون و دیستروفی عضلانی است."
                ],
                "معلولیت بینایی": [
                    "معلولیت بینایی شامل کوری، کم‌بینایی، آب مروارید، گلوکوم و رتینیت پیگمانتوزا می‌شود.",
                    "تکنولوژی‌های کمکی مانند صفحه‌خوان‌ها و نرم‌افزارهای بزرگنمایی می‌توانند کمک کنند."
                ],
                "معلولیت شنوایی": [
                    "معلولیت شنوایی شامل کم شنوایی، کر و لالی، ناشنوایی عصبی و هدایتی می‌شود.",
                    "زبان اشاره، لب‌خوانی و سمعک از روش‌های ارتباطی هستند."
                ],
                "اوتیسم": [
                    "اوتیسم یا اختلال طیف اوتیسم (ASD) یک اختلال رشدی است که بر ارتباط اجتماعی، ارتباطات و رفتار تأثیر می‌گذارد.",
                    "هر کودک اوتیسم منحصر به فرد است و نیازهای خاص خود را دارد."
                ],
                "خدمات نگین": [
                    "خدمات ما شامل آموزش ویژه، گفتاردرمانی، کاردرمانی، فیزیوتراپی، آموزش مهارت‌های ارتباطی، ارتباط تصویری، ارتباط جایگزین، حمایت از خانواده‌ها و وسایل کمکی می‌شود."
                ],
                "چگونه کمک کنم": [
                    "شما می‌توانید از طریق پشتیبانی مالی، اهدای وسایل آموزشی، همکاری تخصصی، داوطلبی یا همکاری سازمانی به ما کمک کنید.",
                    "هر همکاری می‌تواند یک فرصت تازه برای یک کودک باشد."
                ],
                "تماس با نگین": [
                    "شما می‌توانید با شماره ۰۷۸۶۸۳۸۰۰۲ تماس بگیرید یا به ایمیل negineducationcenter@gmail.com پیام ارسال کنید.",
                    "آدرس ما: کابل، پروژهٔ وزیرآباد، سرک ۳۷، افغانستان"
                ],
                "آدرس نگین": ["کابل، پروژهٔ وزیرآباد، سرک ۳۷، افغانستان"],
                "شماره تلفن": ["۰۷۸۶۸۳۸۰۰۲"],
                "ایمیل نگین": ["negineducationcenter@gmail.com"],
                "ساعات کاری": ["شنبه تا چهارشنبه: ۸ صبح تا ۴ بعدازظهر، پنجشنبه: ۸ صبح تا ۱۲ ظهر"],
                "بنیانگذاران": [
                    "اسدالله حیدری و ساحل حیدری بنیان‌گذاران مرکز نگین هستند.",
                    "اجمیر خان میرزاد نیز مشاور ارشد و حامی کلیدی مرکز است."
                ],
                "چرا نگین": [
                    "نگین برای پر کردن خلأ فرصت‌های آموزشی و توان‌بخشی برای کودکان دارای معلولیت ایجاد شد.",
                    "ما باور داریم که تفاوت دلیل محرومیت نیست."
                ],
                "دسترسی‌پذیری": [
                    "وبسایت ما کاملا با ویژگی‌های دسترسی‌پذیری طراحی شده است.",
                    "شما می‌توانید از گزینه‌های تغییر اندازه فونت، حالت تیره و کنتراست بالا استفاده کنید."
                ],
                "ممنون": ["خوشحالم که توانستم کمک کنم! 💎", "برای سوالات بیشتر در خدمت شما هستم."],
                "مرسی": ["خوشحالم که توانستم کمک کنم! 💎", "برای سوالات بیشتر در خدمت شما هستم."],
                "": ["لطفا سوال خود را واضح‌تر بیان کنید.", "من اینجا هستم تا به سوالات شما درباره معلولیت و مرکز نگین پاسخ دهم."]
            };

            function addBotMessage(message) {
                const messageDiv = document.createElement('div');
                messageDiv.classList.add('chatbot-message', 'bot');
                messageDiv.textContent = message;
                chatbotMessages.appendChild(messageDiv);
                chatbotMessages.scrollTop = chatbotMessages.scrollHeight;
            }

            function addUserMessage(message) {
                const messageDiv = document.createElement('div');
                messageDiv.classList.add('chatbot-message', 'user');
                messageDiv.textContent = message;
                chatbotMessages.appendChild(messageDiv);
                chatbotMessages.scrollTop = chatbotMessages.scrollHeight;
            }

            function showTyping() {
                const typingDiv = document.createElement('div');
                typingDiv.classList.add('chatbot-message', 'bot');
                typingDiv.id = 'typing-indicator';
                typingDiv.innerHTML = '<div class="chatbot-typing"><span></span><span></span><span></span></div>';
                chatbotMessages.appendChild(typingDiv);
                chatbotMessages.scrollTop = chatbotMessages.scrollHeight;
            }

            function removeTyping() {
                const typingIndicator = document.getElementById('typing-indicator');
                if (typingIndicator) {
                    typingIndicator.remove();
                }
            }

            function getBotResponse(userMessage) {
                const normalizedMessage = userMessage.toLowerCase().trim();
                
                for (const [key, responses] of Object.entries(chatbotKnowledge)) {
                    if (normalizedMessage.includes(key)) {
                        return responses[Math.floor(Math.random() * responses.length)];
                    }
                }
                
                return chatbotKnowledge[''][Math.floor(Math.random() * chatbotKnowledge[''].length)];
            }

            function handleUserMessage() {
                const message = chatbotInput.value.trim();
                if (!message) return;

                addUserMessage(message);
                chatbotInput.value = '';
                showTyping();

                setTimeout(() => {
                    removeTyping();
                    const response = getBotResponse(message);
                    addBotMessage(response);
                }, 1000);
            }

            if (chatbotToggle && chatbotPopup && chatbotClose && chatbotInput && chatbotSend) {
                chatbotToggle.addEventListener('click', () => {
                    chatbotPopup.classList.toggle('active');
                });

                chatbotClose.addEventListener('click', () => {
                    chatbotPopup.classList.remove('active');
                });

                chatbotSend.addEventListener('click', (e) => {
                    e.preventDefault();
                    handleUserMessage();
                });

                chatbotInput.addEventListener('keypress', (e) => {
                    if (e.key === 'Enter') {
                        e.preventDefault();
                        handleUserMessage();
                    }
                });
            }

            // =====================================================
            // FORM VALIDATION
            // =====================================================
            const contactForm = document.getElementById('contactForm');
            if (contactForm) {
                contactForm.addEventListener('submit', function(e) {
                    e.preventDefault();
                    
                    const name = document.getElementById('name').value.trim();
                    const phone = document.getElementById('phone').value.trim();
                    const message = document.getElementById('message').value.trim();

                    if (!name || !phone || !message) {
                        showToast('لطفاً تمام فیلدهای اجباری را پر کنید.');
                        return;
                    }

                    if (!/^[۰-۹0-9\s\-\+\(\)]+$/.test(phone)) {
                        showToast('لطفاً یک شماره تلفن معتبر وارد کنید.');
                        return;
                    }

                    showToast('پیام شما با موفقیت ارسال شد. به زودی با شما تماس خواهیم گرفت.');
                    contactForm.reset();
                    // Note: Form will submit to FormSubmit.co
                });
            }

            // =====================================================
            // GAME FUNCTIONS
            // =====================================================
            window.checkAnswer = function(number) {
                const message = document.getElementById('gameMessage');
                if (number === 3) {
                    message.innerHTML = '🎉 آفرین! پاسخ درست است.';
                    message.style.color = 'var(--success)';
                    if ('speechSynthesis' in window) {
                        const speech = new SpeechSynthesisUtterance('آفرین! پاسخ درست است.');
                        speech.lang = 'fa-AF';
                        window.speechSynthesis.speak(speech);
                    }
                } else {
                    message.innerHTML = '🌱 دوباره تلاش کنید.';
                    message.style.color = 'var(--orange)';
                    if ('speechSynthesis' in window) {
                        const speech = new SpeechSynthesisUtterance('دوباره تلاش کنید.');
                        speech.lang = 'fa-AF';
                        window.speechSynthesis.speak(speech);
                    }
                }
            };

            // =====================================================
            // LIBRARY FILTER
            // =====================================================
            window.filterLibrary = function(type, button) {
                document.querySelectorAll('.library-filter button').forEach(btn => {
                    btn.classList.remove('active');
                });
                button.classList.add('active');

                document.querySelectorAll('.library-item').forEach(item => {
                    if (type === 'all' || item.dataset.type === type) {
                        item.style.display = '';
                    } else {
                        item.style.display = 'none';
                    }
                });
            };

            // =====================================================
            // SEARCH FUNCTIONS
            // =====================================================
            window.searchSite = function(event) {
                event.preventDefault();
                const input = document.getElementById('searchInput');
                const value = input.value.trim().toLowerCase();

                if (!value) {
                    showToast('لطفاً عبارت مورد نظر را وارد کنید.');
                    return;
                }

                const sections = ['education', 'games', 'videos', 'library', 'parents'];
                let found = false;

                sections.forEach(id => {
                    const section = document.getElementById(id);
                    if (section && section.innerText.toLowerCase().includes(value)) {
                        section.scrollIntoView({ behavior: 'smooth' });
                        found = true;
                    }
                });

                if (found) {
                    showToast('نتیجه جستجو پیدا شد.');
                } else {
                    showToast('نتیجه‌ای برای این جستجو پیدا نشد.');
                }
            };

            window.startVoiceSearch = function() {
                const SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;
                if (!SpeechRecognition) {
                    showToast('جستجوی صوتی در این مرورگر پشتیبانی نمی‌شود.');
                    return;
                }

                const recognition = new SpeechRecognition();
                recognition.lang = 'fa-AF';
                recognition.interimResults = false;
                recognition.start();
                showToast('🎙️ لطفاً صحبت کنید...');

                recognition.onresult = function(event) {
                    const text = event.results[0][0].transcript;
                    const searchInput = document.getElementById('searchInput');
                    if (searchInput) {
                        searchInput.value = text;
                        showToast('عبارت صوتی دریافت شد: ' + text);
                    }
                };

                recognition.onerror = function() {
                    showToast('در دریافت صدای شما مشکلی ایجاد شد.');
                };
            };

            // =====================================================
            // TOAST NOTIFICATION
            // =====================================================
            let toastTimer;
            window.showToast = function(message) {
                const toast = document.getElementById('toast');
                toast.textContent = message;
                toast.classList.add('show');
                clearTimeout(toastTimer);
                toastTimer = setTimeout(() => {
                    toast.classList.remove('show');
                }, 3000);
            };

            // =====================================================
            // SMOOTH SCROLL FOR ANCHOR LINKS
            // =====================================================
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function(e) {
                    const href = this.getAttribute('href');
                    if (href !== '#') {
                        e.preventDefault();
                        const target = document.querySelector(href);
                        if (target) {
                            target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                            // Close mobile menu if open
                            if (navLinks.classList.contains('active')) {
                                navLinks.classList.remove('active');
                                mobileMenuBtn.setAttribute('aria-expanded', 'false');
                            }
                            // Close sidebar on mobile if open
                            if (window.innerWidth <= 992 && sidebar.classList.contains('active')) {
                                sidebar.classList.remove('active');
                                sidebarToggle.setAttribute('aria-expanded', 'false');
                            }
                        }
                    }
                });
            });

            // =====================================================
            // KEYBOARD NAVIGATION
            // =====================================================
            document.addEventListener('keydown', function(e) {
                if (e.ctrlKey && e.key === 'm') {
                    e.preventDefault();
                    document.getElementById('main-content').focus();
                }
                if (e.key === 'Escape') {
                    // Close chatbot with Escape
                    if (chatbotPopup.classList.contains('active')) {
                        chatbotPopup.classList.remove('active');
                        chatbotInput.focus();
                    }
                    // Close sidebar with Escape
                    if (sidebar.classList.contains('active')) {
                        sidebar.classList.remove('active');
                        sidebarToggle.setAttribute('aria-expanded', 'false');
                    }
                }
            });
        });

        // =====================================================
        // TEXT TO SPEECH
        // =====================================================
        function speak(text) {
            if ('speechSynthesis' in window) {
                const speech = new SpeechSynthesisUtterance(text);
                speech.lang = 'fa-AF';
                window.speechSynthesis.speak(speech);
            }
        }
    </script>
</body>
</html>
