<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Volupta® | A cinta que veste sua confiança</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #8B5CF6;
            --secondary: #EC4899;
            --dark: #1F2937;
            --light: #F9FAFB;
            --gray: #6B7280;
            --success: #10B981;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background: #FFFFFF;
        }

        /* Header Banner */
        .banner-top {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            text-align: center;
            padding: 12px 20px;
            font-weight: 500;
            animation: slideDown 0.5s ease;
        }

        @keyframes slideDown {
            from { transform: translateY(-100%); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        /* Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 40px;
            background: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .logo {
            font-size: 24px;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
        }

        .nav-links {
            display: flex;
            gap: 30px;
            list-style: none;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--primary);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
            padding: 60px 20px;
            text-align: center;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 48px;
            color: var(--dark);
            margin-bottom: 20px;
            line-height: 1.2;
        }

        .hero-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
            margin: 40px 0;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .hero-gallery img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .hero-gallery img:hover {
            transform: scale(1.05);
        }

        .rating {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            margin: 20px 0;
            font-size: 18px;
        }

        .stars {
            color: #FCD34D;
        }

        /* Product Section */
        .product-section {
            max-width: 600px;
            margin: 0 auto;
            padding: 40px 20px;
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.1);
        }

        .badge {
            display: inline-block;
            background: var(--secondary);
            color: white;
            padding: 8px 16px;
            border-radius: 50px;
            font-weight: 600;
            margin-bottom: 20px;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }

        .product-title {
            font-size: 28px;
            color: var(--dark);
            margin: 20px 0;
        }

        .product-description {
            color: var(--gray);
            margin-bottom: 30px;
            font-size: 16px;
        }

        .price-section {
            background: linear-gradient(135deg, #F3F4F6 0%, #E5E7EB 100%);
            padding: 30px;
            border-radius: 12px;
            margin: 30px 0;
        }

        .original-price {
            text-decoration: line-through;
            color: var(--gray);
            font-size: 18px;
            margin-bottom: 10px;
        }

        .discount {
            color: var(--secondary);
            font-weight: 700;
            font-size: 16px;
            margin-bottom: 10px;
        }

        .current-price {
            font-size: 36px;
            color: var(--primary);
            font-weight: 700;
            margin-bottom: 10px;
        }

        .payment-options {
            color: var(--gray);
            font-size: 14px;
            margin-top: 10px;
        }

        /* Combo Box */
        .combo-box {
            background: linear-gradient(135deg, rgba(139, 92, 246, 0.1) 0%, rgba(236, 72, 153, 0.1) 100%);
            padding: 20px;
            border-radius: 12px;
            margin: 20px 0;
            border: 2px solid var(--primary);
        }

        .combo-box h3 {
            color: var(--primary);
            margin-bottom: 15px;
            font-size: 18px;
        }

        .combo-box p {
            color: var(--gray);
            margin-bottom: 15px;
        }

        .selector-group {
            margin-bottom: 20px;
        }

        .selector-group label {
            display: block;
            font-weight: 600;
            margin-bottom: 10px;
            color: var(--dark);
        }

        .color-options, .size-options {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
            gap: 10px;
        }

        .option {
            padding: 12px;
            border: 2px solid #E5E7EB;
            border-radius: 8px;
            cursor: pointer;
            text-align: center;
            transition: all 0.3s;
            font-weight: 500;
        }

        .option:hover {
            border-color: var(--primary);
            background: var(--light);
        }

        .option.selected {
            background: var(--primary);
            color: white;
            border-color: var(--primary);
        }

        /* Benefits Section */
        .benefits {
            max-width: 1000px;
            margin: 60px auto;
            padding: 40px 20px;
        }

        .benefits h2 {
            text-align: center;
            font-size: 36px;
            margin-bottom: 50px;
            color: var(--dark);
        }

        .benefits-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }

        .benefit-card {
            background: white;
            padding: 30px;
            border-radius: 12px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0,0,0,0.08);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .benefit-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
        }

        .benefit-number {
            font-size: 48px;
            color: var(--primary);
            font-weight: 700;
            margin-bottom: 15px;
        }

        .benefit-card h3 {
            color: var(--dark);
            margin-bottom: 15px;
            font-size: 20px;
        }

        .benefit-card p {
            color: var(--gray);
            line-height: 1.6;
        }

        /* Comparison Section */
        .comparison {
            background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
            padding: 60px 20px;
            margin: 60px 0;
        }

        .comparison h2 {
            text-align: center;
            font-size: 36px;
            margin-bottom: 50px;
            color: var(--dark);
        }

        .comparison-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            max-width: 900px;
            margin: 0 auto;
            align-items: center;
        }

        .comparison-image {
            border-radius: 12px;
            overflow: hidden;
        }

        .comparison-image img {
            width: 100%;
            display: block;
        }

        .comparison-text h3 {
            font-size: 24px;
            color: var(--dark);
            margin-bottom: 20px;
        }

        .comparison-text p {
            color: var(--gray);
            margin-bottom: 15px;
            line-height: 1.8;
        }

        /* How to Use Section */
        .how-to {
            max-width: 1000px;
            margin: 60px auto;
            padding: 40px 20px;
        }

        .how-to h2 {
            text-align: center;
            font-size: 36px;
            margin-bottom: 50px;
            color: var(--dark);
        }

        .steps {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }

        .step {
            text-align: center;
        }

        .step-number {
            width: 60px;
            height: 60px;
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 28px;
            font-weight: 700;
            margin: 0 auto 20px;
        }

        .step h3 {
            font-size: 18px;
            color: var(--dark);
            margin-bottom: 10px;
        }

        .step p {
            color: var(--gray);
        }

        /* Testimonials Section */
        .testimonials {
            background: white;
            padding: 60px 20px;
        }

        .testimonials h2 {
            text-align: center;
            font-size: 36px;
            margin-bottom: 50px;
            color: var(--dark);
        }

        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .testimonial-card {
            background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
            padding: 30px;
            border-radius: 12px;
            border-left: 4px solid var(--primary);
            transition: transform 0.3s;
        }

        .testimonial-card:hover {
            transform: translateX(5px);
        }

        .testimonial-stars {
            color: #FCD34D;
            margin-bottom: 15px;
            font-size: 16px;
        }

        .testimonial-text {
            color: var(--gray);
            margin-bottom: 20px;
            font-style: italic;
            line-height: 1.6;
        }

        .testimonial-author {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .author-avatar {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: var(--primary);
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 700;
        }

        .author-info h4 {
            color: var(--dark);
            margin-bottom: 2px;
        }

        .author-info p {
            color: var(--gray);
            font-size: 12px;
        }

        /* CTA Button */
        .cta-button {
            display: inline-block;
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            padding: 16px 40px;
            border: none;
            border-radius: 50px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
            text-decoration: none;
            margin: 20px 0;
        }

        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(139, 92, 246, 0.3);
        }

        .cta-button-secondary {
            background: white;
            color: var(--primary);
            border: 2px solid var(--primary);
        }

        .cta-button-secondary:hover {
            background: var(--primary);
            color: white;
        }

        /* Countdown */
        .countdown {
            background: linear-gradient(135deg, var(--secondary) 0%, #F472B6 100%);
            color: white;
            padding: 20px;
            border-radius: 12px;
            text-align: center;
            margin: 20px 0;
            font-weight: 600;
        }

        .countdown-timer {
            font-size: 24px;
            font-weight: 700;
            margin-top: 10px;
            font-family: 'Courier New', monospace;
        }

        /* Trust Section */
        .trust-section {
            background: linear-gradient(135deg, #F9FAFB 0%, #F3F4F6 100%);
            padding: 50px 20px;
            margin: 60px 0;
        }

        .trust-grid {
            max-width: 1000px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40
