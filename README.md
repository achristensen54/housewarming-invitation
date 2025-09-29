
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Housewarming Invitation</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@400;600;700&display=swap');
        
        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(5deg); }
        }
        
        @keyframes spin {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        
        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }
        
        body {
            margin: 0;
            padding: 20px;
            background: linear-gradient(135deg, #ff6b35 0%, #f7931e 25%, #fdc830 50%, #f37335 75%, #ff6b35 100%);
            background-size: 400% 400%;
            animation: gradientShift 15s ease infinite;
            font-family: 'Poppins', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }
        
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .invitation {
            background: linear-gradient(135deg, #fff8e7 0%, #ffe4b5 100%);
            max-width: 650px;
            padding: 60px 50px;
            border-radius: 25px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.3);
            text-align: center;
            position: relative;
            border: 5px solid #ff6b35;
            overflow: hidden;
        }
        
        .invitation::before {
            content: '🍂';
            position: absolute;
            top: -20px;
            left: -20px;
            font-size: 4em;
            opacity: 0.3;
            animation: spin 20s linear infinite;
        }
        
        .invitation::after {
            content: '🍁';
            position: absolute;
            bottom: -20px;
            right: -20px;
            font-size: 4em;
            opacity: 0.3;
            animation: spin 15s linear infinite reverse;
        }
        
        .leaves {
            font-size: 3em;
            margin: 0 0 20px 0;
            animation: float 3s ease-in-out infinite;
        }
        
        .subtitle {
            font-size: 1.3em;
            color: #d2691e;
            letter-spacing: 3px;
            margin-bottom: 15px;
            text-transform: uppercase;
            font-weight: 600;
        }
        
        .main-title {
            font-family: 'Dancing Script', cursive;
            font-size: 4em;
            background: linear-gradient(45deg, #ff6b35, #f7931e, #ff4500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            font-weight: 700;
            margin: 20px 0;
            line-height: 1.2;
            animation: pulse 2s ease-in-out infinite;
        }
        
        .hosts {
            font-size: 1.5em;
            color: #ff6b35;
            font-weight: 700;
            margin: 30px 0 20px 0;
            letter-spacing: 2px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
        }
        
        .details {
            font-size: 1.2em;
            color: #8b4513;
            line-height: 1.8;
            margin: 20px 0;
            font-weight: 600;
        }
        
        .date-time {
            font-size: 1.4em;
            font-weight: 700;
            color: #ff4500;
            margin: 20px 0;
            padding: 20px;
            background: rgba(255, 107, 53, 0.1);
            border-radius: 15px;
            border: 3px dashed #ff6b35;
        }
        
        .message {
            font-size: 1.1em;
            color: #8b4513;
            margin: 30px auto;
            max-width: 500px;
            line-height: 1.8;
            font-weight: 500;
        }
        
        .gift-note {
            font-style: italic;
            font-size: 1.3em;
            color: #ff6b35;
            margin: 30px 0 15px 0;
            font-weight: 700;
        }
        
        .wishlist {
            font-size: 1em;
            color: #8b4513;
            margin-top: 15px;
            font-weight: 500;
        }
        
        .wishlist a {
            color: #ff4500;
            text-decoration: none;
            font-weight: 700;
            padding: 10px 20px;
            background: rgba(255, 107, 53, 0.15);
            border-radius: 10px;
            display: inline-block;
            margin-top: 10px;
            transition: all 0.3s ease;
        }
        
        .wishlist a:hover {
            background: rgba(255, 107, 53, 0.3);
            transform: scale(1.05);
        }
        
        .decoration {
            font-size: 4em;
            margin: 30px 0;
            display: flex;
            justify-content: center;
            gap: 20px;
        }
        
        .decoration span {
            display: inline-block;
            animation: float 2s ease-in-out infinite;
        }
        
        .decoration span:nth-child(2) {
            animation-delay: 0.3s;
        }
        
        .decoration span:nth-child(3) {
            animation-delay: 0.6s;
        }
        
        .fall-banner {
            background: linear-gradient(90deg, #ff6b35, #fdc830, #ff6b35);
            height: 10px;
            width: 100%;
            position: absolute;
            top: 0;
            left: 0;
        }
        
        .fall-banner-bottom {
            background: linear-gradient(90deg, #ff6b35, #fdc830, #ff6b35);
            height: 10px;
            width: 100%;
            position: absolute;
            bottom: 0;
            left: 0;
        }
    </style>
</head>
<body>
    <div class="invitation">
        <div class="fall-banner"></div>
        <div class="fall-banner-bottom"></div>
        
        <div class="leaves">🍂 🍁 🎃</div>
        
        <div class="subtitle">Join us for a</div>
        
        <div class="main-title">Housewarming<br>Celebration</div>
        
        <div class="hosts">ALEX & LAURA CHRISTENSEN</div>
        
        <div class="details">
            🏡 4445 Atlanta Drive, Plano, TX 75093
        </div>
        
        <div class="date-time">
            📅 SATURDAY, OCTOBER 18TH<br>
            🕕 6:30 PM
        </div>
        
        <div class="message">
            We've moved into our new home and it wouldn't feel complete without celebrating with friends and family! Come help us warm our new place with laughter, joy, and great memories! 🏠✨
        </div>
        
        <div class="decoration">
            <span>🎃</span>
            <span>🌻</span>
            <span>🍂</span>
        </div>
        
        <div class="gift-note">
            No gifts necessary!
        </div>
        
        <div class="wishlist">
            But if you feel inclined, we've put together a wish list here:<br>
            <a href="https://tinyurl.com/ALHWwishlist" target="_blank">🎁 View Our Wishlist</a>
        </div>
    </div>
</body>
</html>
