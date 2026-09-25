<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MixPet Shop — Personalised Pet Accessories (EMEA)</title>
    <!-- Google Fonts & Font Awesome Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #FF5A5F;
            --primary-hover: #E0484D;
            --secondary: #00A699;
            --dark: #222222;
            --light-bg: #F7F7F7;
            --white: #FFFFFF;
            --gray: #717171;
            --border: #EBEBEB;
            --radius: 16px;
            --shadow: 0 8px 30px rgba(0,0,0,0.08);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Plus Jakarta Sans', sans-serif;
        }

        body {
            background-color: var(--light-bg);
            color: var(--dark);
            line-height: 1.6;
        }

        /* Top Notification Bar */
        .top-bar {
            background-color: var(--dark);
            color: var(--white);
            text-align: center;
            padding: 8px 16px;
            font-size: 0.85rem;
            font-weight: 600;
        }
        .top-bar span { color: #FFD166; }

        /* Header Navigation */
        header {
            background: var(--white);
            border-bottom: 1px solid var(--border);
            sticky: top;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 16px 24px;
        }
        .logo {
            font-size: 1.5rem;
            font-weight: 800;
            color: var(--primary);
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        .nav-links {
            display: flex;
            gap: 24px;
            list-style: none;
        }
        .nav-links a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 600;
            font-size: 0.95rem;
            transition: color 0.2s;
        }
        .nav-links a:hover { color: var(--primary); }
        .nav-actions {
            display: flex;
            align-items: center;
            gap: 16px;
        }
        .region-badge {
            background: #E8F5E9;
            color: #2E7D32;
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 700;
            display: flex;
            align-items: center;
            gap: 6px;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #FFF5F5 0%, #E6FFFA 100%);
            padding: 60px 24px;
            text-align: center;
        }
        .hero-container {
            max-width: 800px;
            margin: 0 auto;
        }
        .hero h1 {
            font-size: 2.8rem;
            font-weight: 800;
            line-height: 1.2;
            margin-bottom: 16px;
        }
        .hero p {
            font-size: 1.1rem;
            color: var(--gray);
            margin-bottom: 24px;
        }

        /* Main Container & Grid */
        .main-container {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 24px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
        }

        @media (max-width: 850px) {
            .main-container { grid-template-columns: 1fr; }
            .hero h1 { font-size: 2rem; }
        }

        /* Card Styles */
        .card {
            background: var(--white);
            border-radius: var(--radius);
            padding: 32px;
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
        }
        .card-title {
            font-size: 1.4rem;
            font-weight: 700;
            margin-bottom: 8px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .card-subtitle {
            font-size: 0.9rem;
            color: var(--gray);
            margin-bottom: 24px;
        }

        /* 3D Personalization Studio */
        .preview-box {
            background: radial-gradient(circle, #f0f0f0 0%, #e0e0e0 100%);
            height: 240px;
            border-radius: 12px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            position: relative;
            margin-bottom: 20px;
            perspective: 1000px;
            overflow: hidden;
        }
        .pet-tag-3d {
            width: 140px;
            height: 140px;
            background: linear-gradient(145deg, #ffd700, #b8860B);
            border-radius: 50%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: #333;
            box-shadow: 0 10px 20px rgba(0,0,0,0.2), inset 0 2px 5px rgba(255,255,255,0.8);
            transform-style: preserve-3d;
            transition: transform 0.1s ease-out;
            border: 4px solid #daa520;
        }
        .tag-hole {
            width: 14px;
            height: 14px;
            background: #d0d0d0;
            border-radius: 50%;
            position: absolute;
            top: 12px;
            box-shadow: inset 0 2px 4px rgba(0,0,0,0.4);
        }
        .tag-text-name {
            font-size: 1.2rem;
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: 1px;
            text-shadow: 1px 1px 0px rgba(255,255,255,0.4);
            margin-top: 10px;
        }
        .tag-text-phone {
            font-size: 0.75rem;
            font-weight: 700;
            opacity: 0.8;
        }

        /* Form Controls */
        .form-group {
            margin-bottom: 16px;
        }
        .form-group label {
            display: block;
            font-size: 0.85rem;
            font-weight: 700;
            margin-bottom: 6px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }
        .form-control {
            width: 100%;
            padding: 12px 16px;
            border: 2px solid var(--border);
            border-radius: 10px;
            font-size: 0.95rem;
            transition: border-color 0.2s;
        }
        .form-control:focus {
            outline: none;
            border-color: var(--primary);
        }

        .btn {
            display: inline-block;
            width: 100%;
            background-color: var(--primary);
            color: var(--white);
            border: none;
            padding: 14px 20px;
            font-size: 1rem;
            font-weight: 700;
            border-radius: 10px;
            cursor: pointer;
            transition: background 0.2s, transform 0.1s;
            text-align: center;
        }
        .btn:hover { background-color: var(--primary-hover); }
        .btn:active { transform: scale(0.98); }

        /* Pet Species Selector */
        .species-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 10px;
            margin-bottom: 16px;
        }
        .species-option {
            border: 2px solid var(--border);
            border-radius: 10px;
            padding: 12px;
            text-align: center;
            cursor: pointer;
            transition: all 0.2s;
        }
        .species-option:hover, .species-option.active {
            border-color: var(--secondary);
            background-color: #E6FFFA;
        }
        .species-option i {
            font-size: 1.4rem;
            color: var(--secondary);
            margin-bottom: 4px;
            display: block;
        }
        .species-option span {
            font-size: 0.8rem;
            font-weight: 700;
        }

        /* VIP Pricing Cards */
        .vip-card {
            background: linear-gradient(135deg, #1A1A1A 0%, #333333 100%);
            color: var(--white);
            border-radius: var(--radius);
            padding: 24px;
            margin-top: 30px;
            position: relative;
            overflow: hidden;
        }
        .vip-card::after {
            content: "PAWS CLUB VIP";
            position: absolute;
            right: -20px;
            bottom: -10px;
            font-size: 2.5rem;
            font-weight: 900;
            opacity: 0.05;
            color: var(--white);
        }
        .vip-price {
            font-size: 1.8rem;
            font-weight: 800;
            color: #FFD166;
            margin: 10px 0;
        }

        /* Mixpanel Debug Console */
        .analytics-console {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 24px;
        }
        .console-box {
            background: #1E1E1E;
            color: #4AF626;
            font-family: monospace;
            padding: 20px;
            border-radius: 12px;
            height: 200px;
            overflow-y: auto;
            font-size: 0.85rem;
        }
        .console-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 10px;
            color: var(--white);
            font-size: 0.9rem;
            font-weight: 700;
        }
    </style>
</head>
<body>

    <!-- Top Promo Bar -->
    <div class="top-bar">
        <span>Midsummer EMEA Flash Sale!</span> Use code <strong>SUMMER26</strong> for 20% off + Free Engraving!
    </div>

    <!-- Header Navigation -->
    <header>
        <div class="nav-container">
            <a href="#" class="logo">
                <i class="fa-solid fa-paw"></i> MixPet Shop
            </a>
            <ul class="nav-links">
                <li><a href="#studio">3D Custom Studio</a></li>
                <li><a href="#profile">Pet Profile</a></li>
                <li><a href="#vip">Paws Club VIP</a></li>
            </ul>
            <div class="nav-actions">
                <div class="region-badge">
                    <i class="fa-solid fa-globe"></i> UK & Ireland (EMEA)
                </div>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-container">
            <h1>Bespoke Pet Accessories, Tailored for Your Best Friend.</h1>
            <p>Premium laser-engraved collars, harnesses, and ceramic feeders across EMEA. Interactive 3D preview guaranteed.</p>
        </div>
    </section>

    <!-- Main Application Grid -->
    <div class="main-container">

        <!-- Column 1: Interactive 3D Engraving Personalization Studio -->
        <div class="card" id="studio">
            <div class="card-title">
                <i class="fa-solid fa-cube" style="color: var(--primary);"></i>
                3D Engraving Studio
            </div>
            <div class="card-subtitle">Personalize your brass tag with live interactive 3D rotation.</div>

            <!-- 3D Tag Preview Box -->
            <div class="preview-box" id="previewBox">
                <div class="pet-tag-3d" id="petTag">
                    <div class="tag-hole"></div>
                    <i class="fa-solid fa-dog" style="font-size: 1.5rem; margin-top: 10px;"></i>
                    <div class="tag-text-name" id="previewName">MAX</div>
                    <div class="tag-text-phone" id="previewPhone">+44 7911 123456</div>
                </div>
            </div>

            <!-- Inputs -->
            <div class="form-group">
                <label>Pet Name</label>
                <input type="text" id="inputName" class="form-control" value="MAX" maxlength="12">
            </div>
            <div class="form-group">
                <label>Emergency Phone Number</label>
                <input type="text" id="inputPhone" class="form-control" value="+44 7911 123456">
            </div>
            <div class="form-group">
                <label>Promo Code</label>
                <input type="text" id="inputPromo" class="form-control" value="WELCOME10">
            </div>

            <button class="btn" id="btnAddToCart">
                <i class="fa-solid fa-cart-shopping"></i> Add Custom Tag to Cart (€25.00)
            </button>
        </div>

        <!-- Column 2: Pet Profile & VIP Subscription -->
        <div>
            <!-- Pet Profile Builder -->
            <div class="card" id="profile">
                <div class="card-title">
                    <i class="fa-solid fa-id-card" style="color: var(--secondary);"></i>
                    Build Your Pet Profile
                </div>
                <div class="card-subtitle">Complete your profile to unlock custom breed recommendations.</div>

                <div class="form-group">
                    <label>Select Pet Species</label>
                    <div class="species-grid">
                        <div class="species-option active" onclick="selectSpecies('Dog')">
                            <i class="fa-solid fa-dog"></i>
                            <span>Dog</span>
                        </div>
                        <div class="species-option" onclick="selectSpecies('Cat')">
                            <i class="fa-solid fa-cat"></i>
                            <span>Cat</span>
                        </div>
                        <div class="species-option" onclick="selectSpecies('Rabbit & Small Pet')">
                            <i class="fa-solid fa-otter"></i>
                            <span>Small Pet</span>
                        </div>
                    </div>
                </div>

                <div class="form-group">
                    <label>Breed Size</label>
                    <select class="form-control" id="breedSize">
                        <option value="Small">Small (e.g., French Bulldog, Pug)</option>
                        <option value="Medium" selected>Medium (e.g., Beagle, Cocker Spaniel)</option>
                        <option value="Large">Large (e.g., Golden Retriever, German Shepherd)</option>
                    </select>
                </div>

                <button class="btn" style="background-color: var(--secondary);" id="btnSaveProfile">
                    <i class="fa-solid fa-check"></i> Save Pet Profile
                </button>
            </div>

            <!-- VIP Subscription Card -->
            <div class="vip-card" id="vip">
                <div style="font-size: 0.85rem; font-weight: 700; color: #FFD166; text-transform: uppercase;">Exclusive Loyalty</div>
                <h3 style="font-size: 1.5rem; margin-top: 4px;">Paws Club VIP Membership</h3>
                <div class="vip-price">€4.99 <span style="font-size: 0.9rem; color: #ccc;">/ month</span></div>
                <ul style="list-style: none; font-size: 0.9rem; margin-bottom: 20px; line-height: 1.8;">
                    <li><i class="fa-solid fa-check" style="color: #4AF626;"></i> Free Express Shipping across all EMEA</li>
                    <li><i class="fa-solid fa-check" style="color: #4AF626;"></i> Free 3D Custom Laser Engraving</li>
                    <li><i class="fa-solid fa-check" style="color: #4AF626;"></i> Annual Free Birthday Gift Box</li>
                </ul>
                <button class="btn" style="background-color: #FFD166; color: var(--dark);" id="btnJoinVIP">
                    Subscribe to Paws Club VIP
                </button>
            </div>
        </div>

    </div>

    <!-- Mixpanel Analytics Live Debug Console -->
    <div class="analytics-console">
        <div class="console-header">
            <span><i class="fa-solid fa-terminal"></i> Mixpanel Event Dispatcher (Live Debugging)</span>
            <span style="font-size: 0.75rem; color: #aaa;">Super Properties Loaded: Country, Platform, Channel</span>
        </div>
        <div class="console-box" id="consoleLog">
            [System initialized] Mixpanel Tracker Ready. Listening for user actions...<br>
        </div>
    </div>

    <!-- JavaScript Logic & Mixpanel Mocking -->
    <script>
        // Mixpanel Super Properties State
        const superProperties = {
            country: "United Kingdom",
            emea_sub_region: "UK & Ireland",
            platform: "Web Storefront",
            marketing_channel: "Instagram Ads",
            membership_status: "Guest / Unregistered"
        };

        // Mock Mixpanel Track Function
        function mixpanelTrack(eventName, properties = {}) {
            const eventPayload = {
                event: eventName,
                properties: {
                    ...superProperties,
                    ...properties,
                    time: new Date().toISOString()
                }
            };

            const consoleBox = document.getElementById('consoleLog');
            consoleBox.innerHTML += `<br><span style="color: #FFD166;">[MIX-PANEL TRACK]</span> <strong>${eventName}</strong>: ` + JSON.stringify(eventPayload.properties);
            consoleBox.scrollTop = consoleBox.scrollHeight;
            console.log("Mixpanel Event Dispatched:", eventPayload);
        }

        // 3D Tag Rotation Effect
        const previewBox = document.getElementById('previewBox');
        const petTag = document.getElementById('petTag');

        previewBox.addEventListener('mousemove', (e) => {
            const rect = previewBox.getBoundingClientRect();
            const x = e.clientX - rect.left - (rect.width / 2);
            const y = e.clientY - rect.top - (rect.height / 2);
            petTag.style.transform = `rotateY(${x * 0.2}deg) rotateX(${-y * 0.2}deg)`;
        });

        previewBox.addEventListener('mouseleave', () => {
            petTag.style.transform = `rotateY(0deg) rotateX(0deg)`;
        });

        // Real-time Tag Text Update
        const inputName = document.getElementById('inputName');
        const inputPhone = document.getElementById('inputPhone');
        const previewName = document.getElementById('previewName');
        const previewPhone = document.getElementById('previewPhone');

        inputName.addEventListener('input', (e) => {
            previewName.textContent = e.target.value.toUpperCase() || 'NAME';
        });

        inputPhone.addEventListener('input', (e) => {
            previewPhone.textContent = e.target.value || 'PHONE';
        });

        // Interactive Species Selector
        let selectedPetSpecies = 'Dog';
        function selectSpecies(species) {
            selectedPetSpecies = species;
            document.querySelectorAll('.species-option').forEach(el => el.classList.remove('active'));
            event.currentTarget.classList.add('active');
        }

        // Button Event Handlers + Analytics Dispatching
        document.getElementById('btnAddToCart').addEventListener('click', () => {
            // Track Personalization Applied First
            mixpanelTrack('Personalization Applied', {
                customization_type: "Laser Engraved Name & Phone",
                preview_mode_used: "3D_Interactive",
                pet_name_length: inputName.value.length
            });

            // Track Item Added to Cart
            mixpanelTrack('Item Added to Cart', {
                pet_type: selectedPetSpecies,
                accessory_category: "Bespoke Engraved Collars & Tags",
                bundle_type: "Individual Item",
                promo_code: document.getElementById('inputPromo').value
            });

            alert('Customized Engraved Tag added to your cart!');
        });

        document.getElementById('btnSaveProfile').addEventListener('click', () => {
            mixpanelTrack('Pet Profile Created', {
                pet_species: selectedPetSpecies,
                breed_size: document.getElementById('breedSize').value,
                pet_profile_completeness: "Complete Profile"
            });

            alert('Pet Profile successfully saved!');
        });

        document.getElementById('btnJoinVIP').addEventListener('click', () => {
            // Upgrade user super property
            superProperties.membership_status = "Subscriber (Paws Club VIP)";

            mixpanelTrack('VIP Club Subscribed', {
                billing_cycle: "Monthly (€4.99)",
                membership_tier: "Paws Club VIP"
            });

            alert('Welcome to Paws Club VIP!');
        });

        // Trigger Page View on Load
        window.addEventListener('DOMContentLoaded', () => {
            mixpanelTrack('Product Catalog Browsed', {
                filter_applied: "Personalized Only"
            });
        });
    </script>
</body>
</html>
